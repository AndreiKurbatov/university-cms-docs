<!DOCTYPE html>
<html>

<body> 
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
	<h4>General information</h4> 
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
	<h4>TO DO<h4>
		<ol>
			<li>Create a student<li> <!---->
			<li>Update a student<li> <!---->
			<li>Find a studen by id<li> <!---->
			<li>Find a student by the passport id<li> <!---->
			<li>Find all students<li> <!---->
			<li>find all students related to a group by group's name<li> <!---->
			<li>Find all students related to a course by course's name<li> <!---->
			<li>Find all students related to a teacher by teacher's name<li> <!---->
			<li>Find all students by student's specialization<li> <!---->
			<li>Find a student by name<li> <!---->
			<li>Delete a student from a group by group's id<li>
			<li>Delete a student from a course by course's id<li>
			<li>Delete a student by id<li>
			<li>Assign a student to a group by group's name<li>
			<li>Assign a student to a course by course's name<li>
		</ol>
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
		<li>An administrator can assign a student to a course or a group or can move a student to another group or a course.</li>
		<li>An administrator can create a post to publish it on home page</li>
		<li>An administrator can see a schedule of all users and change it</li>
		<li>During the creation/modification of the schedule, it should be taken into account that the teacher has a working shift, it is impossible to assign lectures for the teacher during non-working hours</li>
		<li>The schedule is generated for one semester</li>
		<li>An administrator can see all groups and courses and create new ones</li>
	</ul>
	<br>
	<h2>Menu description</h2>
	<br>
	<h3>The given user is logged on as a <b>'Student'</b></h3>
	<ul>
		<li>User on the homepage</li>
		<li>On the homepage user can see news from the university</li>
		<li>The user can see the <b>'Navigation menu'</b> on the homepage
			<ul>
				<li>The user can see and navigate <b>'Navigation menu' -> 'Registered Courses'</b> menu</li>
				<li>The user should see the list of student's courses</li>
				<ul>
					<li>The user can select specific <b>'Navigation menu' -> 'Registered Courses' -> 'Course'</b>
							from the list</li>
					<li>The user should see course specific information </li>
				</ul>
				<li>User can see and navigate to <b>'Navigation menu' -> 'My Schedule'</b> menu</li>
				<li>The user should see student's schedule according with selected date/range filter</li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'My group'</b> menu</li>
				<li>The user should see group's specific information </li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Profile'</b> menu</li>
				<li>The user should see student specific information</li>
			</ul>
		</li>
	</ul>
	<br>
	<h3>The given user is logged on as a <b>'Teacher'</b></h3>
	<ul>
		<li>User on the homepage</li>
		<li>On the homepage user can see news from the university</li>
		<li>The user can see the <b>'Navigation menu'</b> on the homepage
			<ul>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'My Schedule'</b> menu</li>
				<li>The user should see student's schedule according with selected date/range filter</li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Profile'</b> menu</li>
				<li>The user should see teacher specific information</li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'My Courses'</b> menu</li>
				<li>The user should see all courses for current teacher
					<ul>
						<li>The user can see and navigate to specific <b>'Navigation menu' -> 'My Courses' ->
								'Course'</b>menu</li>
						<li>The user can add books or comments to the course description</li>
				</li>
			</ul>
		</li>
	</ul>
	</li>
	</ul>
	<br>
	<h3>The given user is logged on as a 'administrator'</h3>
	<ul>
		<li>User on the homepage</li>
		<li>On the homepage user can see news from the university</li>
		<li>The user can see the <b>'Navigation menu'</b> on the homepage
			<ul>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Create a post '</b> menu</li>
				<li>The user can create a post and publish it on the homepage</li>
		</li>
		<li>The user can see and navigate to <b>'Navigation menu' -> 'Manage schedule'</b> menu</li>
		<li>The user should see the list of teachers and list of courses they teach
			<ul>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Manage schedule' -> 'Teacher'</b></li>
				<li>The user should see the schedule for the specific teacher and can make changes</li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Manage schedule' -> 'Student'</b></li>
				<li>The user should see the schedule for the specific student and can make changes</li>
			</ul>
		</li>
		<li>The user can see and navigate to <b>'Navigation menu' -> 'Groups'</b> menu</li>
		<li>The user can see the list of all groups and get information about groups using filter by name/id
			<ul>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Groups' -> 'Create Group'</b> menu</li>
				<li>The user can create a new group</li>
			</ul>
		</li>
		<li>The user can see and navigate to <b>'Navigation menu' -> 'Courses'</b> menu</li>
		<li>The user can see the list of all groups and get information about groups using filter by name/id
			<ul>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Courses' -> 'Create course'</b> menu</li>
				<li>The user can create a new course</li>
			</ul>
		</li>
	</ul>
</body>

</html>