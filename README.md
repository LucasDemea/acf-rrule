# ACF RRule Field

Create recurring rules within a single ACF field and retrieve all the dates using the [simshaun/recurr](https://github.com/simshaun/recurr) package.

![ACF RRule Screenshot](https://pixelparfait.fr/_github/acf-rrule.png)

## Usage

```
<?php $rrule = get_field('rrule'); ?>
```

The RRule field returns an array with the following arguments:

**rrule** *(string)*  
The RRule string for your recurring rule  

**start_date** *(string)*  
The start date for the recurrence  

**start_time** *(string)*  
The start time for the recurrence  

**frequency** *(string)*  
The frequency for the recurrence (DAILY, WEEKLY, MONTHLY or YEARLY)  

**interval** *(int)*  
The interval set for the frequency   

**weekdays** *(array)*  
An array of days for the weekly frequency  

**monthdays** *(array)*  
An array of days for the monthly frequency  

**months** *(array)*  
An array of months for the yearly frequency  

**monthly_by** *(string)*  
The selected option between "monthdays" and "setpos" for the monthly frequency  

**bysetpos** *(array)*  
The starting numbers for the monthly "setpos" option  

**byweekday** *(array)*  
The selected days for the monthly "setpos" option  

**end_type** *(string)*  
The end of the recurrence between "date" and "count"  

**end_date** *(string)*  
The end date in YYYYMMDD format for the recurrence when `end_type` is set to "date"  

**occurence_count** *(int)*  
The number of occurences for the recurrence when `end_type` is set to "count"  

**dates_collection** *(array)*  
An array containing all the DateTime objects generated by your recurring rule  

**text** *(string)*  
A text representation for your recurring rule  
