<!DOCTYPE html>
<html>

<body> 
	<h2>Entity description</h2>
	<h3>CourseTime</h3>
	<ul>
		<li>A <b>CourseTime</b> has
			<ol>
				<li>course course time </li> 
				<li>course date</li> 
				<li>course start time</li> 
				<li>course end time </li> 
			</ol>
		</li>
		<li><b>CourseTime</b> is used to create <b>'Courses schedule'</b></li>
		<li>A student cannot change the timetable, only see it</li>
		<li>A student can see only its own time table</li>
	</ul>
	<br>
	<h3>Course</h3> 
	<ul>
		<li>A <b>Course</b> has:
			<ol>
				<li>course id</li> 
				<li>teacher id</li> 
				<li>specialization</li> 
				<li>course name</li> 
				<li>credit hours</li> 
				<li>course description</li> 
				<li>course date </li> 
				<li>start time</li> 
				<li>end time</li> 
				<li>class room</li> 
			</ol>
		</li>
		<li>A student can attend only courses related to his specialization</li>
		<li>Students attends from 10 to 15 Courses</li>
		<li>There are 80 courses in total at the university</li>
		<li>For a student to attend a course, it is not necessary for him to be in a group</li>
	</ul>
	<br>
	<h3>Group</h3>  
	<ul>
		<li>A <b>Group</b> has:
			<ol>
				<li>group id</li> 
				<li>group name</li> 
				<li>specialization</li> 
			</ol>
		</li>
		<li>Each group has a specialization: Computer Science (20 courses),<br>
			Medicine (20 courses), Economics (20 courses) or Art (20 courses)</li>
		<li>A group contains from 15 to 30 students</li>
		<li>There are 107 groups in total</li>
		<li>The group name must consist of two uppercase<br>
			Latin letters followed by a hyphen followed by two digits</li>
	</ul>
	<br>
	<h3>Student</h3> 
	<ul>
		<li>A <b>Student</b> has:
			<ol>
				<li>student id</li> 
				<li>group id</li> 
				<li>first name</li> 
				<li>last name</li> 
				<li>date of birth</li> 
				<li>passport number</li> 
				<li>scholarship amount</li> 
				<li>currency name</li>
				<li>telephone number</li>
				<li>email address</li> 
				<li>residence address</li>
				<li>admission date</il> 
				<li>specialization</li> 
				<li>current semester</li> 
				<li>person foto</il> 
			</ol>
		</li>
		<li>For a student to attend a course, it is not necessary for him to be in a group</li>
		<li>It is possible that there is a group without students or a student without group</li>
		<li>There are 3200 students in total at the university</li>
		<li>A student has a group and courses</li>
		<li>A group contains from 15 to 30 students</li>
		<li>Students attends from 10 to 15 Courses</li>
		<li>There are 4 years of study. That is there are 8 semesters.<br>
		The 1st year contains 800 students, the 2st year contains 800 students,<br>
		the 3th year contains 800 students and the 4th year contains 800 students</li>
		<li>A student can see its courses</li>
		<li>A student can see its group</li>
		<li>A student has a schedule of courses and final tests but cannot change it</li>
		<li>A student can see its payment information but cannot change it</li>
	</ul>
	<br>
	<h3>Teacher</h3> 
	<ul>
		<li>A <b>Teacher</b> has:
			<ol>
				<li>teacher id</li> 
				<li>first name</li> 
				<li>last name</li> 
				<li>date of birth</li> 
				<li>salary amount</li> 
				<li>currency name</li>
				<li>employment date</li> 
				<li>position</li> 
				<li>passport number</li> 
				<li>telephone number</li> 
				<li>email address</li> 
				<li>residence address</li> 
				<li>working shift</li> 
				<li>scientific degree</li>
				<li>person foto</il> 
			</ol>
		</li>
		<li>A teacher teaches one or more courses </li>
		<li>A teacher can see its schedule</li>
		<li>A teacher can access its profile</li>
	</ul>
	<br>
	<h3>Administration</h3> 
	<ul>
		<li>An <b>Administration</b> has:
			<ol>
				<li>administrator id</li> 
				<li>first name</li> 
				<li>last name</li> 
				<li>date of birth</li>
				<li>employment date</li> 
				<li>salary amount</li> 
				<li>currency name</li>
				<li>position</li> 
				<li>telephone number</li> 
				<li>email address</li> 
				<li>residence address</li> 
				<li>passport number</li> 
				<li>working shift</li> 
				<li>person foto</il> 
			</ol>
		</li>
		<li>An administrator can assign a student to a course<br>
			or a group or can move a student to another group or<br>
			a course.</li>
		<li>An administrator can create a post to publish it on home page</li>
		<li>An administrator can see a schedule of all users and change it</li>
		<li>During the creation /modification of the schedule, it should be taken into account<br>
		 that the teacher has a working shift, it is impossible to assign lectures for the teacher<br>
		 during non-working hours</li>
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