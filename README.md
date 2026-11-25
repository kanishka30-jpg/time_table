# Ex04 Time Table
# Date: 25-11-2026
# AIM
To write a html webpage page to display your slot timetable.

# ALGORITHM
## STEP 1
Create a Django-admin Interface.

## STEP 2
Create a static folder and inert HTML code.

## STEP 3
Create a simple table using `<table>` tag in html.

## STEP 4
Add header row using `<th>` tag.

## STEP 5
Add your timetable using `<td>` tag.

## STEP 6
Execute the program using runserver command.

# PROGRAM
```
<!DOCTYPE html>
<html>
<head>
    <title>Slot Timetable</title>

    <style>
    

.timetable th {
    background-color: black;
    color: white;
}

.timetable td {
    background-color: #eeeeee;
    color: black;
}

.timetable tr:nth-child(even) td {
    background-color: #f5dce5;
}

.timetable td.day {
    background-color: #e8a3bd;
    color: black;
    font-weight: bold;
}

.timetable tr:nth-child(even) td.day {
    background-color: #e8a3bd;
}
.timetable {
    width: 90%;
    margin: 0 auto 20px auto;
    border: 4px solid #777;
    border-collapse: collapse;
}

.subject-table {
    width: 90%;
    margin: 20px auto;
    border: 4px solid #777;
    border-collapse: collapse;
}

.subject-table th,
.subject-table td {
    border: 2px solid #777;
    padding: 10px;
}

.subject-table th,
.subject-table td {
    border: 2px solid #777;
    padding: 8px;
}

.subject-table th {
    text-align: center;
    background-color: #eeeeee;
}

.subject-table td:first-child,
.subject-table td:nth-child(2) {
    text-align: center;
}

.subject-table td:last-child {
    text-align: left;
}
.subject-table th,
.subject-table td {
    border: 2px solid grey;
    padding: 10px;
}

.subject-table th {
    text-align: center;
    background-color: #eeeeee;
}

.subject-table td {
    text-align: left;
}

.subject-table {
    border-collapse: collapse;
}
.timetable {
    border: 3px solid black;
}
.timetable th,
.timetable td{
    border: 2px solid black;
}
.vertical {
    writing-mode: horizontal-tb;
    text-align: center;
    vertical-align: middle;
    line-height: 1.1;
}
body { margin: 8px; }
h3 { margin-top: 5px; font-size: 16px; }
table th, table td {
    padding: 4px 8px;
    font-size: 14px;
}
.vertical { font-size: 12px; line-height: 1.1; }
    </style>

</head>

<body>
    <center>
      <img src="saveetha_logo.png" width="450">
    </center>
    
    <h3 style="text-align:center; margin-bottom:0;">
    SLOT TIMETABLE - KANISHKA M (26006227)
    </h3>
    <table class="timetable">
        <tr>
            <th>Day/time</th>
            <th>8.00 t0 9.30 AM</th>
            <th>9.45 to 11.15 AM</th>
            <th>11.30 to 12.15 PM</th>
            <th>12.30 to 1.00 PM</th>
            <th>1.15 to 2.45 PM</th>
            <th>3.00 to 4.30 PM</th>
        </tr>

        <tr>
            <td><b>Monday</b></td>
            <td>FWAD</td>
            <td>Python Programming</td>
            <td class="vertical" rowspan="5">
            M<br>E<br>N<br>T<br>O<br>R<br>
            M<br>E<br>E<br>T
            </td>
            <td class="vertical" rowspan="6">
            L<br>U<br>N<br>C<br>H
            </td>
            <td>Free Slot</td>
            <td>Free Slot</td>
        </tr>

        <tr>
            <td><b>Tuesday</b></td>
            <td>FWAD</td>
            <td>EDM</td>
            <td>FCC</td>
            <td>Free Slot</td>
        </tr>

        <tr>
            <td><b>Wednesday</b></td>
            <td>Python Programming</td>
            <td>Free Slot</td>
            <td>Free Slot</td>
            <td>Free Slot</td>
        </tr>

        <tr>
            <td><b>Thursday</b></td>
            <td>Python Programming</td>
            <td>CA</td>
            <td>FCC</td>
            <td>EDM</td>
        </tr>

        <tr>
            <td><b>Friday</b></td>
            <td>CDS</td>
            <td>Free Slot</td>
            <td>Free Slot</td>
            <td>Free Slot</td>
        </tr>

        <tr>
            <td><b>Saturday</b></td>
            <td>CA</td>
            <td>BEEE</td>
            <td>Free Slot</td>
            <td>FWAD</td>
            <td>Free Slot</td>
        </tr>
    </table>

    <table class="subject-table">
        <tr>
            <th>S.No</th>
            <th>Subject Code</th>
            <th>Subject Name</th>
        </tr>

        <tr>
            <td>1.</td>
            <td>19AI414</td>
            <td>Fundamentals of Web Application Development (FWAD)</td>
        </tr>

        <tr>
            <td>2.</td>
            <td>19AI301</td>
            <td>Python Programming(PP)</td>
        </tr>

        <tr>
            <td>3.</td>
            <td>19AI302</td>
            <td>Engineering Design and Modelling (EDM)</td>
        </tr>
        <tr>
            <td>4.</td>
            <td>19CS547</td>
            <td>Fundamentals of Cryptocurrency(FCC)</td>
        </tr>
        <tr>
            <td>5.</td>
            <td>19CS305</td>
            <td>Computer Architecture(CA)</td>
        </tr>
        <tr>
            <td>6.</td>
            <td>19EY708</td>
            <td>Career Development Skills(CDS)</td>
        </tr>
        <tr>
            <td>7.</td>
            <td>19EE305</td>
            <td>Basic Electrical, Electronics and Measurement Engineering(BEEE)</td>
        </tr>

    </table>

</body>
</html>
```
# OUTPUT
<img width="1895" height="873" alt="Screenshot 2026-11-25 204727" src="https://github.com/user-attachments/assets/d0125a02-f9b0-44a4-be38-17b2251110c7" />


# RESULT
The program for creating slot timetable using basic HTML tags is executed successfully.
