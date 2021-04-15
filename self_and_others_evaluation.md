<h1 align="center"><b>SELF & OTHER'S EVALUATION</b></h1>
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
    <a href="#OBJECTIVE">Objective</a>
    </li>
    <li>
    <a href="#How Did I Write My Formulae">How Did I Write My Formulae</a>
    </li>
    <li>
    <a href="#TEST CASES">Test Cases</a>
    </li>
    <li>
    <a href="#How It Was Implemented">How It Was Implemented?</a>
    </li>
    <li>
    <a href="#Explanation of Implementation">Explanation of Implementation</a>
    </li>
    <li>
    <a href="#Test Results">Test Results</a>
    </li>
    <li>
    <a href="#Conclusions">Conclusions</a>
    </li>
    <li>
    <a href="#Contact">Contact</a>
    </li>
  </ol>  
</details>

## OBJECTIVE:
The objective for **Self & Other's Evaluation** project was to evaluate every person on the basis of their past performance in this course.

After evaluating every person by the words *excellent-5, very good-4, good-3, satisfactory-2, fair-1 and poor 0*, the average of their points were to be displayed in a seperate column.

For the extra task, the objective was to put a red color in the row if the person had earned less than 2.5 average score.

## How Did I Write My Formulae:
I wrote my formula by using **vlookup** and **avg** functions.

My formulae were:

    For Calling Data =VLOOKUP(B4,Copy!B3:K3,10)
    For Average =Avg(C3:J3)

## TEST CASES:
|Trial|Description|Result|
|-----|-----------|------|
|Adding Individual category|First I tried to segregate all the elements like good and fair, then summing them up individually for every name and adding the total, then dividing it by total no. to get the average.|The test result was **SUCCESSFULL**, but the whole process was a lot complex and time consuming|
|Calling Values| I tried to call all the values individually in a copy sheet and then taking out their average in the same copy sheet. I basically pulled the value from skills chart to copy sheet and pushed average column from copy sheet to skills chart which was much easier to do and also worked properly on real time basis.|The test result was **SUCCESSFULL** and also it was much easier to implement.|

---
---
## How Was It Implemented?

Basically the whole idea was to make the whole spreadsheet as simple as possible. So when my mind was out of ideas to think of a formula that could directly find the average of the students, I created a seperate spreadsheet and named it "**COPY**".

<img align="center" src="https://user-images.githubusercontent.com/55484239/114871556-088fa480-9e17-11eb-8f33-26c8a372a36c.JPG" />

I pushed all the data from the original spreadsheet i.e. **Skills Chart** to the copy spreadsheet and got the values in the same. Then I calculated the averages of all the students with a simple function "**=avg**" and pushed all the data to the original spreadsheet which made it to work in real time basis.

After using this formula I have used conditional formating tool. With the help of this we can set a range of value so that if the value got down as per selected range then the color of perticular row or column will change.

<img align="center" src="https://user-images.githubusercontent.com/55484239/114886883-92df0500-9e25-11eb-92d3-1791955a8d89.JPG" />

## Explanation of Implementation:
The whole idea was to find a formula to calculate the avg of the students. The challenge for me was to change the array to an intger without actually showing it in the spreadsheet. The method was very simple, let me explain it step by step:

1. First of all i created a ""**copy**"" spreadsheet and pushed all the data from skills chart to the copy sheet.
2. Then I changed all the array data to an integer data with the help of function "**=vlookup**".
3. I calculated the average of all the students with the help of "**=avg**" function.
4. At last I pushed all the data from the copy sheet to the original sheet with the help of "**=vlookup**" function.

## Test Results:
The test results were **Satisfactory** as it worked and also changed if edited on real time basis.

### Improvements To Be Made:
1. The formula could have been more simplified.
2. Instead of using an extra spreadsheet, I should have thought for a different idea to make it more simplified.

## Conclusions:
Being a total newbie in this project I atleast completed it with positive results, but the overall spreadsheet could have been more simplified if I gave a little more efforts to think of a formula which worked without using any extra spreadsheets.

The Link for the spreadsheet is mentioned below:

[LINK](https://docs.google.com/spreadsheets/d/1HfmpUI3zo7W3i_ipaRXQ1VQN8SfjfTX1fhow03rY-_Y/edit?usp=sharing)
---
---

Thank You,

**Aayon**

Contact: *aayonmukherjee21@gmail.com*
