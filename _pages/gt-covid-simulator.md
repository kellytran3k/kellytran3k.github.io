---
layout: page
title: GT Covid-19 Simulator
permalink: projects/gt-covid-19-simulator/
subtitle: GT Covid-19 Testing Simulator
---

## A simulator that mimicked the procedures of the Georgia Institute of Technology's Covid-19 testing response system

This simulator is the result of a final group project for **CS 4400** *(Intro to Database Systems).*

The goal of the project was to *fully implement* amd *simulate* the testing procedures used at
**Georgia Tech** during the *COVID-19 pandemic*.

This was done using a mock SQL database to read and update data with **Flask** and **Python3**. **PyMySQL** and **MySQL** workbench was used for the database API and **Anaconda** for the virtual environment.

This system calls from a database to allow faculty and students to:
- view and filter through available testing appointments
- set and update testing appointments
- view and filter through available testing sites
- view individual testing results
- filter and view congregated (pooled) testing results

In addition, lab technicians, site testers, and admins were able to
update data in real time.

Meaningful data includes:
- individual testing results
- pooled testing results
- testing sites
- testing appointments

## Sample Python Code to 'View Daily Results':

```py
@app.route('/view_daily_results', methods=['GET', 'POST'])
def view_daily_results():
    msg = ''
    # connects w database
    cursor = connection.cursor()
    # calls daily_results on database
    cursor.callproc('daily_results')
    connection.commit()

    # fetches the daily results
    cursor.execute('SELECT * FROM daily_results_result')
    resultDetails = cursor.fetchall()

    # returns daily results
    return render_template('view_daily_results.html',
        resultDetails=resultDetails)
```

## Conclusion:

Through this project, I learned the **integration process of SQL database with Python3** in order to develop a web application that updated and retrieved data in real time. This was one of my first times using a **virtual environment** to implement code, as well as using **MySQL** to call datasets. The web application can be functionally run locally. However, there is currently no plan of putting this simulator online.

*Special thank you to: Michael Piseno, Yun Ha Jeon, and Holly M.*

GitHub link: [GT Testing Simulator](https://github.com/kellytran3k/covid-testing-db)
