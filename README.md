# SISE2601 Project data description
### Army Service Within At-Risk Youth
Final project in Advanced Data Analysis in R course

================

Team name - Danielle Eldor, Shir Bernstein and Amit Haritan

This markdown file describes the data folder structure and organization ...

To reproduce the code, add to the current folder the data file “child_risk.sav” and run the code.

The data suggests that childhood adversity and trauma, such as loss, parental issues, maltreatment, and social difficulties, can have long-lasting effects on individuals. These adverse experiences are associated with poor health, behavioral problems, and negative outcomes in adulthood, including mental health issues,  low incomes, and difficulties in education and employment. These effects tend to emerge during young adulthood, a critical phase when individuals transition into adult roles and responsibilities. If protective factors are lacking during childhood and adolescence, young adults who have experienced adverse childhood experiences may struggle to cope with the challenges they face, leading to lower adaptation and potential mental and behavioral dysfunction. The data measures 3 different time period throughout 10 years, of a constant group of at-risk youth.

The element we are trying to predict is whether an at-risk teen will be recruited to the IDF in his or her future. For this, we will use the values of the column T3army, indicating if they got recruited or not, to test and compare to our models

Data feature list (valid features):


# T3Army

This field indicates whether a child serve in the army or not.
Missing values were ignored.

| Value |       Label     |
|:-----:|:---------------:|
|   1   |  Served         |
|   2   |  Did not served |


# Life skils features

There are 5 scales of preparedness to an independent adult life.
All scales set between 1-4 with gaps of 0.25, and each field contains a specific category:

  - M1.2 - education
  - M1.3 - employment
  - M1.4 - housing
  - M1.5 - social relations
  - M1.6 - normative behavior
  
  - B_life_skills_all - summarizes the children's skills of the 2nd measurement (T2).
    This column has continuous values acseding from 1-4.
  
  
# Hopes

There are 6 sentences that show the child's depiction of future struggles and coping in scale of 1-5:

| Value |        Label           |
|:-----:|:----------------------:|
|   1   |   Do not agree at all  |
|   2   |     Low agreement      |
|   3   |    Moderately agree    |
|   4   |     Much agreement     |
|   5   |     Very much agree    |
 

The sentences:

- SenseCont1 - What happens to me may depend mainly on me.
- SenseCont2 - I can do almost anything I set my mind to.
- SenseCont3 - Many times I feel that I cannot deal with my problems in life.
- SenseCont4 - I have little control over the things that happen in my life.
- SenseCont5 - There is no way I can solve the many problems that bother me in life.
- SenseCont6 - I can only slightly change the things that are important to me in life.


Hope1, Hope2  - Fields that indicate a measure of hope for the future.
Hope1 is about the feelings of hope themselves and Hope2 is about patterns of hope.


HopeAll_T1 - summarized the children's hopes of the 1st measurement.


B.EDUCATION - This field indicates the children answer about "What education or certificate do you currently have"? in scale of 1-7:

| Value |        Label           |
|:-----:|:----------------------:|
|   1   |   Partial high school  |
|   2   |   Complete high school |
|   3   |  Partial matriculation |
|   4   | Complete matriculation |
|   5   |   Secondary education  |
|   6   |   Academic education   |
|   7   |         refused        |
                


# Traumas

The next fields contain descriptions of traumatic events that the teens may have experienced during their childhood up to the age of 18. The answers are labeled as following:

| Value |  Label |
|:-----:|:------:|
|   1   |   No   |
|   2   |   Yes  |


The trauma descriptions:

- T3_ACE_1 - Has a parent or other adult in the home often cursed, insulted, humiliated you, or behaved in a way that made you fear you might be physically harmed?
- T3_ACE_2 - Has a parent or other adult at home often physically hurt you (eg, pulled, pushed, dragged, or thrown something at you)? Or left marks of violence on your body?
- T3_ACE_3 - If an adult or a person at least 5 years older than you, held, touched, caressed or made you touch their body sexually? Or forced sexual contact?
- T3_ACE_4 - Have you often felt that no one in your family loved you or thought you were important or special? Or do the family members not support and care for each other?
- T3_ACE_5 - Have you felt that you lack food, clean clothing adapted to the weather, that there is no one to protect you? Or was your parent drunk when you needed them?
- T3_ACE_6 - Have you seen your mother or someone who took care of you beaten or attacked?
- T3_ACE_7 - Did you live with someone who had a drinking problem or who regularly used drugs?
- T3_ACE_8 - Was anyone in the household depressed or mentally ill or tried to commit suicide?
- T3_ACE_9 - Has anyone in the household been in prison?



Hacha1-10 - Fields that are about preparation programs, extracurriculars and plans for the future.
We specifically want to use in Hacha3 and Hacha10.

Hacha3 and Hacha10 are about the army preparation:

 - Hacha3 asks if they got good army preparation.
 
| Value |  Label |
|:-----:|:------:|
|   1   |   No   |
|   2   |   Yes  |

 - Hacha10 is an acsending scale from 1-5 rating the army preparation they received.



# General

- T3gender -  This field contains the children's gender:

| Value |  Label |
|:-----:|:------:|
|   1   |  women |
|   2   |   men  |


- T3religiousness - This field indicates the children's level of religiousness:

| Value |           Label           |
|:-----:|:-------------------------:|
|   1   |       ultra-Orthodox      |
|   2   |         religious         |
|   3   |   Traditional-Religious   |
|   4   | Traditional-low Religious |
|   5   |   Secular, non-religious  |
