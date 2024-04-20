<!DOCTYPE html>
<html>

<body> 
	<h2>Credentials</h2>
	<ul>
		<li>Administrator: login admin,  password 1234</li>
		<li>Student: login userM17, password 1234</li>
		<li>Teacher: login teacherM17, password 1234
	</ul>
	<h2>Entity description</h2>
	<h3>Lesson</h3>
	<ul>
		<li>A lesson is used to create a courses schedule</li>
		<li>A lesson contains information about its student course, room and precise time</li>
		<li>A student or a teacher cannot change the timetable, only see it</li>
		<li>A student as a teacher can see only his own courses schedule</li>
		<li>The courses schedule can be changed only by an administrator</li>
	</ul>
	<br>
	<h3>Room</h3>
	<ul>
		<li>A room contains information about the room number and floor</li>
	<br>
	<h3>Course</h3> 
	<ul>
		<li>A student can attend only courses related to his specialization</li>
		<li>Students attends from 4 to 7 Courses</li>
		<li>There are 40 courses in total at the university:<br>
		Computer Science (10 courses), Medicine (10 courses), Economics (10 courses) Art (10 courses)</li>
		<li>For a student to attend a course, it is not necessary for him to be in a group with relevant specialization</li>
		<li>An administrator can change students in a Course</li>
	</ul>
	<br>
	<h3>Group</h3>  
	<ul>
		<li>Each group has a specialization:<br>Computer Science (10 courses),
			Medicine (10 courses), Economics (10 courses) or Art (10 courses)</li>
		<li>A group contains from 15 to 30 students</li>
		<li>There are 27 groups in total</li>
		<li>The group name must consist of two uppercase Latin letters followed by a hyphen followed by two digits</li>
		<li>An administrator can change students in a group</li>
	</ul>
	<br>
	<h3>Student</h3> 
	<ul>
		<li>For a student to attend a course, it is not necessary for him to be in a group with relevant specialization.<br>
		The student deletion from the group lead to his deletion from all courses</li>
		<li>It is possible that there is a group without students or a student without group</li>
		<li>There are 800 students in total at the university</li>
		<li>A student has a group and courses with relevant specialization</li>
		<li>A group contains from 15 to 30 students</li>
		<li>Students attends from 4 to 7 courses</li>
		<li>A student can see its courses</li>
		<li>A student can see its group</li>
		<li>A student has a list of his courses but cannot change it</li>
		<li>A student can access his profile</li>
	</ul>
	<br>
	<h3>Teacher</h3> 
	<ul>
		<li>A teacher teaches one or more courses </li>
		<li>A teacher can see its schedule</li>
		<li>A teacher can access its profile</li>
		<li>A teacher cannot change information about a group or a course</li>
	</ul>
	<br>
	<h3>Administration</h3> 
	<ul>
		<li>There are 10 administrators</li>
		<li>An administrator can assign a student to a course or a group or can move a student to another group or a course.</li>
		<li>An administrator can create a post to publish it on home page</li>
		<li>An administrator can see a schedule of all users and change it</li>
		<li>During the creation/modification of the schedule, it should be taken into account that the teacher has a working shift, it is impossible to assign lectures for the teacher during non-working hours</li>
		<li>The schedule is generated for one semester</li>
		<li>An administrator can see all groups and courses and create new ones</li>
	</ul>
</body>

</html>