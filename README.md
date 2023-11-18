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
	<h3>Exam</h3> 
	<ul>
		<li>An <b>Exam</b> has:
			<ol>
				<li>exam id</li> 
				<li>teacher id</li> 
				<li>course id</li> 
				<li>exam date</li> 
				<li>exam start time</li> 
				<li>exam end time</li> 
				<li>classroom number</li> 
			</ol>
		</li>
		<li><b>Exam</b> is used to create a <b>'Academic Calendar'</b></li>
		<li>The <b>'Academic Calendar'</b> has information about upcoming exams</li>
		<li>The exams dates can be generated only for the current semester</li>
		<li>The student can only see information about exams related to their courses</li>
		<li>The student cannot change the information about exams</li>
		<li>A student and a teacher can have several exams</li>
		<li>Only a administrator can change information about exams</li>
		<li>A teacher can see the all exams he is involved</li>
	</ul>
	<br>
	<h3>Grade</h3>
	<ul>
		<li>A <b>Grade</b> has:
			<ol>
				<li>grade id</li>
				<li>student id</li> 
				<li>course id</li> 
				<li>grade</li> 
				<li>date</li> 
			</ol>
		</li>
		<li>The <b>Grade</b> is used to create 'Personal Diary'</li>
		<li>A student can see all his grades according to his courses</li>
		<li>A student cannot change grade information</li>
		<li>A teacher can see and change grade information regarding all related students</li>
	</ul>
	<br>
	<h3>Task</h3> 
	<ul>
		<li>A <b>Task</b> has:
			<ol>
				<li>task id</li> 
				<li>student id</li> 
				<li>teacher id</li> 
				<li>course id</li> 
				<li>teacher task file</li>
				<li>student task file</li> 
				<li>published date</li>
				<li>deadline</li> 
				<li>completed marker</li> 
				<li>task description</li>
			</ol>
		</li>
		<li>A task can be created only by a teacher and assigned<br>
			to a student from teacher's course</li>
		<li>A student can see only his tasks</li>
		<li>A teacher can see all tasks of the students associated with him</li>
		<li>A task can be changed by a teacher after publishing</li>
		<li>A student can upload a file as a responce for teacher's task</li>
		<li>A student can change the answer after publishing</li>
		<li>A teacher can mark a task as 'accepted' or 'not accepted'</li>
		<li>A teacher and a student can left a comment to a task</li>
	</ul>
	<br>
	<h3>Payment</h3> 
	<ul>
		<il>A <b>Payment</b> has:
			<ol>
				<li>payment id</li> 
				<li>student id</li> 
				<li>payment number</li>
				<li>semester</li> 
				<li>payment amount </li> 
				<li>next payment date</li> 
				<li>status</li> 
			</ol>
		</il>
		<li>Only the administrator can make payments<br>
		 to the system and see information about them</li>
		<li>Administrator can filter the payments by student id,<br>
		 payment number, semester and status</li>
		 payments of all students</li>
		<li>A student can see only his payments</li>
		<li>A student can filter payments by status</li>
		<li>If the payment date is overdue, an email is send<br>
		 automatically to the student.</li>
		<li>Before the first payment, the payment status<br>
		 is 'no payment'. If the next payment date is overdue,<br>
		 then the status is 'overdue'. If the payment is paid<br>
		 in time then the status is 'accepted'.</li>
	</ul>
	<br>
	<h3>Book</h3> 
	<ul>
		<li>A <b>Book</b> has:
			<ol>
				<li>book id</li> 
				<li>course id</li> 
				<li>book title</li> 
				<li>author(s)</li> 
				<li>edition</li> 
				<li>specialization</li> 
				<li>ISBN</li> 
				<li>publisher</li> 
				<li>url</li> 
			</ol>
		</li>
		<li>A teacher and a student can access books, but only teacher can add a new book to course</li>
		<li>Book information can be changed by a teacher</li>
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
		<li>A student can send a message to a teacher or to a student</li>
		<li>A student can see its grades</li>
		<li>A student can see its payment information but cannot change it</li>
		<li>A student can see its tasks and complete them but cannot add a task by itself</li>
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
		<li>A teacher can see its grade book and see<br>
			grade information about all students regarding the teacher's course</li>
		<li>A teacher can access its profile</li>
		<li>A teacher can create and verify tasks regarding the students of its course</li>
		<li>A teacher can write messages to a student, a teacher or an administrator</li>
		<li>A teacher can see all its courses and add book information and/or left a comment</li>
		<li>A teacher can see dates of the final exams of its course but cannot change it</li>
		<li>A teacher can write an email to a student</li>
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
		<li>An administrator can see all student's payments.</li>
		<li>An administrator can see and send messages to another teacher or administrator</li>
		<li>An administrator can see and and change the dates of final exams of all courses</li>
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
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Academic Calendar'</b> manu</li>
				<li>The user can see dates of final exams</li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'My group'</b> menu</li>
				<li>The user should see group's specific information </li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Personal Diary'</b> manu</li>
				<li>The user should see student's specific grades</li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Account Book'</b> menu</li>
				<li>The user should see information about payments for the student and<br>
					filter payments by type: past payment, upcoming payment, debt</li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Profile'</b> menu</li>
				<li>The user should see student specific information</li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Todo list'</b> menu</li>
				<li>The user should see all task from teachers and filter them by<br>
					course name or teacher name.
					<ul>
						<li>The user can see and navigate to <b>'Navigation menu' -> 'Todo list' -> 'Answer'</b> manu
							of<br>
							the specific task from the Todo list.</li>
						<li>The user can upload .pdf, .word, .odt, png, .txt <br>
							file as a response for the task.</li>
					</ul>
				</li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Message box'</b></li>
				<li>The user can see and send messages to another student or to another teacher</li>
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
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Grade book'</b> manu</li>
				<li>The user should see student's specific grades</li>
				<li>The user should see the all students related to the teacher and all student grades.<br>
					It's possible to find student by name or filter by average grade.</li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Profile'</b> menu</li>
				<li>The user should see teacher specific information</li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Tasks'</b> menu</li>
				<li>The user should see two separate windows: <b>'Completed tasks'</b> (which are marked as
					'accepted')<br>
					and <b>'Uncompleted tasks'</b> (which aren't marked as 'accepted')
					<ul>
						<li>The user can see and navigate to <b>'Navigation menu' -> 'Tasks' -> 'Uncompleted tasks'</b>
							menu</li>
						<li>The user should see the student's response and mark the task as 'accepted' or/and left the
							comment</li>
						<li>The user can see and navigate to <b>'Navigation menu' -> 'Tasks' -> 'Create task'</b> menu
						</li>
						<li>A user can create a task and assign it to one or more students or an entire course.</li>
					</ul>
				</li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Message box'</b> menu</li>
				<li>The user can see and send messages to another student, teacher or administrator</li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'My Courses'</b> menu</li>
				<li>The user should see all courses for current teacher
					<ul>
						<li>The user can see and navigate to specific <b>'Navigation menu' -> 'My Courses' ->
								'Course'</b>menu</li>
						<li>The user can add books or comments to the course description</li>
				</li>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Academic Calendar'</b> manu</li>
				<li>The user can see dates of final exams</li>
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
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Account Book'</b> menu</li>
				<li>The user should see information about all student payments and<br>
				<li>The user can see and navigate to <b>'Navigation menu' -> 'Academic Calendar'</b> manu</li>
				<li>The user can add a date of final exams</li>
				by type: past payment, upcoming payment, debt
		</li>
		<li>The user can see and navigate to <b>'Navigation menu' -> 'Message box'</b></li>
		<li>The user can see and send messages to another teacher or administrator</li>
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