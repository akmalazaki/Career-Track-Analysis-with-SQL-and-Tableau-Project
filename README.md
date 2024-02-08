## **Tableau Link**
https://public.tableau.com/app/profile/akmal.azaki/viz/SQLandTableauProjectSolution-Part3/DashboardCareerTrackAnalysis

## **Case Description**
One of the functionalities the 365 company introduced in a 2021 platform release included the option for student enrollment in a career track. The tracks represent an ordinal sequence of courses that eventually lead to obtaining the skills for one of three job titles: data scientist, data analyst, or business analyst.

Completing a career track on the platform is a challenging task. To acquire a corresponding career certificate, a student must pass nine course exams (seven compulsory and two elective courses) and sit for a career track exam encompassing topics from all seven required courses.

In this Career Track Analysis with SQL and Tableau project, you’re tasked with analyzing the career track enrollments and achievements of 365’s students. You’ll first need to retrieve the necessary information from an SQL database. Afterward, you’ll feed this information to Tableau, visualize the results, and finally interpret them.
***

In this Career Track Analysis with SQL and Tableau project, you’re tasked with analyzing the career track enrollments and completions of 365’s students. You’ll first need to retrieve the necessary information from an SQL database. Afterward, you’ll feed this information to Tableau and visualize the results.

Study the sql_and_tableau database, consisting of the following tables:

**career_track_info**
1. track_id – the unique identification of a track, which serves as the primary key to the table
2. track_name – the name of the track

**career_track_student_enrollments**
1. student_id – the unique identification of a student
2. track_id – the unique identification of a track. Together with the previous column, they make up the primary key to the table—i.e., each student can enroll in a specific track only once. But a student can enroll in more than one career track.
3. date_enrolled – the date the student enrolled in the track. A student can enroll in more than one career track.
4. date_completed – the date the student completed the track. If the track is not completed, the field is NULL.
***

## **Problem Finding**
Based on the analysis results, it was found that the majority of students enrolled in the data analyst program, approximately 49.1%. This percentage is the highest compared to the other two programs, namely data scientist with a registration proportion of about 36.8%, and business analyst with a registration proportion of about 14.1%.

However, students in the data analyst program have the lowest average track_completed, around 22.8%. This figure is the lowest percentage compared to the other two programs.

To answer why this is happening, relevant data for further analysis is needed, such as ratings for each program depicting student satisfaction and other useful relevant data.
