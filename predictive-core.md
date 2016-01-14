
##Institution
* TENANT_ID
* TENANT_NAME

##Student
* [STUDENT_ID](#student_id)
* [ULN](#ULN)
* DOB
* ETHNICITY
* GENDER
* AGE
* LEARN_DIF
* DISABILITY1
* DISABILITY2
* DOMICILE
* TERMTIME_ACCOM
* PARENTS_ED
* SOCIO_EC
* OVERSEAS

##Course
* COURSE_ID
* SUBJECT
* TITLE
* COURSE_AIM

##Course Instance
* COURSE_ID
* COURSE_INSTANCE_ID
* START_DATE
* END_DATE
* ACADEMIC_YEAR

##Student on Course Instance
* STUDENT_ID
* COURSE_INSTANCE_ID
* WITHDRAWAL_REASON
* WITHDRAWAL_DATE
* MODE
* YEAR_COM
* YEAR_PRG
* YEAR_STU
* COURSE_AVERAGE_GRADE
* YEAR_AVERAGE_GRADE
* ENTRY_QUALS
* ENTRY_POINTS
* COURSE_OUTCOME
* COURSE_GRADE

##Module
* MOD_ID
* MOD_NAME
* MOD_SUBJECT
* MOD_CREDITS

##Module Instance
* MOD_ID
* MOD_INSTANCE_ID
* MOD_START_DATE
* MOD_END_DATE
* MOD_PERIOD
* MOD_ONLINE
* MOD_ENROLLMENT
* MOD_ACADEMIC_YEAR
* MOD_OPTIONAL
* MOD_LEVEL

##Student on a module Instance
* STUDENT_ID
* COURSE_INSTANCE_ID
* MOD_INSTANCE_ID
* MOD_OUTCOME
* MOD_GRADE
* MOD_PASS
* MOD_RETAKE

##Grade
* STUDENT_ID
* MOD_INSTANCE_ID
* GRADABLE_OBJECT
* CATEGORY
* MAX_POINTS
* EARNED_POINTS
* WEIGHT
* GRADE_DATE

##Activity
* STUDENT_ID
* MOD_ID
* EVENT
* EVENT_DATE


# Definitions
##STUDENT_ID
###Description

The institution's own unique identifier of the student. In the case or event of requiring to provide anonymous data for trial/ evaluation purposes with JISC, institutions should use a suitable method or algorithm (which can be reversed by that institution, for evaluation purposes thereafter) to ensure that this studentid provided is different to that actual ID held locally.

###Purpose

To identify the student across multiple records within an institution

###Derivation

https://www.hesa.ac.uk/index.php?option=com_studrec&task=show_file&mnl=14051&href=a^_^OWNSTU.html

###References

###Format

String 255

###Compulsory

Yes

###Notes

##ULN
###Description
Unique Learner Number. For initial trial and data model development for the predictive model, this field should be left NULL.

###Purpose
For future use, tracking student journey.

###Derivation
Skills Funding Agency: See https://www.gov.uk/government/publications/lrs-unique-learner-numbers

###References

###Format
String (10)

###Compulsory
No

###Notes
The ULN can be provided as an additional point of reference, however the STUDENT_ID will always take precedence as the unique learner/ student identifier