3D Reconstruction with Computer Vision
--------------------------------------
### CS 378 (53132), Fall 2014

#### Meetings: Tuesdays and Thursdays, 9:30-11am, WEL 2.256
#### Unique number: 53132

### Instructor: [Bryan Klingner](http://cs.utexas.edu/~bmk)
- Email: bmk at cs dot utexas dot edu
- Office hours: Thursday 5-6pm, GDC 5.420

### TA: Pengxiang Cheng
- Email: pxcheng at cs dot utexas dot edu
- Office hours: Tuesday 4-5pm, GDC 1.302 (TA Station) Desk 2

### Course discussion [on Piazza](https://piazza.com/utexas/fall2014/cs378/home)

## Course aims and objectives

Projects like [Photosynth](http://photosynth.net/), [Kinect](http://en.wikipedia.org/wiki/Kinect), and [Tango](https://www.google.com/atap/projecttango/#project) have shown the incredible potential of using computer vision to construct immersive 3D environments from easily acquired imagery. In this lab-based class, we'll dive into practical applications of 3D reconstruction, combining hardware and software to build our own 3D environments from scratch. 

We'll use open-source frameworks like [OpenCV](http://opencv.org/) to do the heavy lifting, with the focus on understanding and applying state-of-the art approaches to geometric computer vision. Along the way, we'll use industry standard revision management tools like [Git](http://git-scm.com/) and [Github](http://github.com). The class will culminate in a final project of your choice that puts your new 3D reconstruction skills to use.

### Specific learning objectives
By the end of the class, you should be able to:
 1. Extract 3D information latent in 2D images and video.
 2. Apply state-of-the-art scientific libraries without needing a full grasp of their implementations.
 3. Use industry standard software engineering practices such as version control and peer code review.

## Class format
The class will be heavily project-based. Projects will be completed in small groups. I'll assign early projects with specific goals and evaluations. Your group will design the final project, which will occupy roughly the last third of the semester. 

We'll devote lots of in-class time to working on projects with the TA and I available to help. Each class may begin with a short presentation on a topic relevant to the current assignment. You should expect to spend time outside of class gaining additional background and practice with the topics covered by the projects.

## Course Schedule
This schedule is a living thing and may change as needed to accomodate the class's progress.

|  # | Date |     | Topic     | Details   | Reading | Projects |
|---:|------|:---:|-----------| ----------|---------|----------|
|  1 | Thursday 28 Aug | <img width="400" src="https://raw.githubusercontent.com/ut-cs378-vision-2014fall/course-info/master/images/lena_pixels.png"/> | [Introductions and image basics](https://github.com/ut-cs378-vision-2014fall/course-info/raw/master/meeting-notes/01_28_august.pdf) | We meet each other. I'll tell you what I hope cover, you'll tell me what you hope to learn. | 2.1, 2.3 | Project 0 out |
|  2 | Tuesday 2 Sep | <img width="400" src="https://raw.githubusercontent.com/ut-cs378-vision-2014fall/course-info/master/images/image_alignment.png"/> | [Image Alignment 1](https://github.com/ut-cs378-vision-2014fall/course-info/raw/master/meeting-notes/02_02_sept.pdf) | Image warping | 3.6.1  |  |
|  3 | Thursday 4 Sep | <img width="400" src="https://raw.githubusercontent.com/ut-cs378-vision-2014fall/course-info/master/images/image_alignment.png"/> | [Image Alignment 2](https://github.com/ut-cs378-vision-2014fall/course-info/raw/master/meeting-notes/03_04_sept.pdf) | Fitting a model | 6.1.1, 6.1.4 | Project 0 due Project 1 out |
|  4 | Tuesday 9 Sep | <img width="400" src="https://raw.githubusercontent.com/ut-cs378-vision-2014fall/course-info/master/images/feature_match.png"/> | [Feature Matching 1](https://github.com/ut-cs378-vision-2014fall/course-info/raw/master/meeting-notes/04_09_sept.pdf) | What is an interest point? What is a feature? | 4.1.1-3 | |
|  5 | Thursday 11 Sep | <img width="400" src="https://raw.githubusercontent.com/ut-cs378-vision-2014fall/course-info/master/images/feature_match.png"/> | [Feature Matching 2](https://github.com/ut-cs378-vision-2014fall/course-info/raw/master/meeting-notes/05_11_sept.pdf) | Invariant features and feature matching | 4.1.1-3 | |
|  6 | Tuesday 16 Sep | <img width="400" src="https://raw.githubusercontent.com/ut-cs378-vision-2014fall/course-info/master/images/poisson_blend.png"/> | [Image Blending](https://github.com/ut-cs378-vision-2014fall/course-info/raw/master/meeting-notes/06_16_sept.pdf) | High-level overview of blending | 3.5, 9.3, [Burt & Adelson](http://www.cs.princeton.edu/courses/archive/fall05/cos429/papers/burt_adelson.pdf) | |
|  7 | Thursday 18 Sep | <img width="400" src="https://raw.githubusercontent.com/ut-cs378-vision-2014fall/course-info/master/images/stereo.png"/> | [Stereo 1](https://github.com/ut-cs378-vision-2014fall/course-info/raw/master/meeting-notes/07_18_sept.pdf) | Epipolar geometry | 11.1 | |
|  8 | Tuesday 23 Sep | <img width="400" src="https://raw.githubusercontent.com/ut-cs378-vision-2014fall/course-info/master/images/stereo.png"/> | [Stereo 2](https://github.com/ut-cs378-vision-2014fall/course-info/raw/master/meeting-notes/08_23_sept.pdf) | Epipolar review + Project 1 Worktime | | Project 1 due |
|  9 | Thursday 25 Sep | <img width="400" src="https://raw.githubusercontent.com/ut-cs378-vision-2014fall/course-info/master/images/stereo.png"/> | [Stereo 3](https://github.com/ut-cs378-vision-2014fall/course-info/raw/master/meeting-notes/09_25_sept.pdf) | Computing disparity / Code Review | | Project 1 code reviews out |
| 10 | Tuesday 30 Sep | <img width="400" src="https://raw.githubusercontent.com/ut-cs378-vision-2014fall/course-info/master/images/sfm_thumb.png"/> | [Structure from Motion 1](https://github.com/ut-cs378-vision-2014fall/course-info/raw/master/meeting-notes/10_30_sept.pdf) | Project 1 recap, SfM intro, Project 2  | | Project 2 out |
| 11 | Thursday 2 Oct | <img width="400" src="https://raw.githubusercontent.com/ut-cs378-vision-2014fall/course-info/master/images/sfm_thumb.png"/> | [Structure from Motion 2](https://github.com/ut-cs378-vision-2014fall/course-info/raw/master/meeting-notes/11_02_oct.pdf) | Street View SfM | | Project 1 code reviews due |
| 12 | Tuesday 7 Oct | <img width="400" src="https://raw.githubusercontent.com/ut-cs378-vision-2014fall/course-info/master/images/stereo_proj.png"/> | Project 2 work week     |  | |  |
| 13 | Thursday 9 Oct | <img width="400" src="https://raw.githubusercontent.com/ut-cs378-vision-2014fall/course-info/master/images/stereo_proj.png"/> | Project 2 work week     |  | |  |
| 14 | Tuesday 14 Oct | | Video 1     | Motion  | | Project 2 due |
| 15 | Thursday 16 Oct | | Video 2      | Action Recognition | | Project 2 code reviews due Friday 17 Oct |
| 16 | Tuesday 21 Oct  | | Video 3      | Tracking | | Project 2 Revisions due. Project 3 out |
| 17 | Thursday 21 Oct  | | Applications 1      |  | |  |
| 18 | Tuesday 28 Oct  | | Applications 2      |  | | Final project groups and proposals due |
| 19 | Thursday 30 Oct | | Industry guest lecture | Chris Slaughter, Lynx Labs | |
| 20 | Tuesday 4 Nov | | Final Project Work | On-demand topics | | Project 3 due, Final project proposal evaluations back |
| 21 | Thursday 6 Nov | | Final Project Work | On-demand topics  |  | |
| 22 | Tuesday 11 Nov | | Final Project Work | On-demand topics | | Final project progress report 1 due |
| 23 | Thursday 13 Nov | | Final Project Work | On-demand topics |  | |
| 24 | Tuesday 18 Nov | | Final Project Work | On-demand topics |  | |
| 25 | Thursday 20 Nov | | Final Project Work | On-demand topics | | Final project progress report 2 due |
| 26 | Tuesday 25 Nov | | Final Project Presentations 1 | |  | | 
| 27 | Tuesday 2 Dec | | Final Project Presentations 2 | | | Final projects due |
| 28 | Thursday 4 Dec | | Final Project Presentations 3 | |  | |

## Topic overview

### Image basics
- Programming environment (Python/Numpy/OpenCV)
- Revision control with Git
- Code submission, and peer review with Github
- Digital image representation
- Basic image transformations

### Image features
- What is an interest point?
- How can we summarize image appearance?
- Matching features

### Multiple views of a scene
- Camera models
- Homography
- RANSAC
- Image warping
- Stitching

### Stereo and Structure From Motion
- Stereo vision
- Camera motion
- Triangulation
- Track formation

### Real-time 3D tracking
- Object segmentation
- Motion estimation
- Scene estimation


## Course requirements

### Prerequisites
- Basic knowledge of probability, statistics, and linear algebra.
- Strong programming experience. Projects will be completed in Python. While no previous Python experience is required, I expect you to learn the Python you need to complete your assignments on your own outside of class.
- No specific experience with computer vision is required.

### Attendance and Participation
Classtime will be largely devoted to working in small groups, when you'll have access to me and the TA. While attendance is not required, it's to your advantage to come to collaborate with your group and stay abreast of developments in the course schedule.

### Course materials

You'll find the following resources useful:
- Computer Vision: Algorithms and Applications, by Rick Szeliski. [Free online](http://szeliski.org/Book/) or [buy at Amazon](http://www.amazon.com/Computer-Vision-Algorithms-Applications-Science/dp/1848829345/).
- [OpenCV Python Tutorials](http://docs.opencv.org/trunk/doc/py_tutorials/py_tutorials.html)

### Grading

Grades will be based on a series of projects completed in small groups. Projects will be due about every two weeks. I'll assign different groups of three students for each of projects 0-3, and you can choose your own group of 3-4 students for the final project 4, which will be on a topic of your choosing.

Each project will be graded in three phases:
1. Initial code submission (80%)
2. Peer code review (10%)
3. Revised code submission (10%)

See the project pages for details on submission and grading phases.

Here is a list of the five projects for the class, along with *estimated* due dates. Actual dates may vary to accomodate class progress.

| Name | Description | Weight | Due date (estimated) |
|------|-------------|--------|----------------------|
| Project 0 | Account setup and image basics | 10% | 4 Sept |
| Project 1 | Stitching a panorama | 20% | 23 Sept |
| Project 2 | Dense stereo reconstruction | 20% | 14 Oct |
| Project 3 | Real-time tracking | 20% | 4 Nov |
| Project 4 | Choose your own adventure! | 30% | 2 Dec | 

### Late policy
Submit your project by 11:59 PM on the day that its due according to the project's instructions.

You're allowed three late days to use at your discretion across the semester with no penalty to your grade. If you submit your assignment any later than 11:59 on its due date, you will consume a late day. After all three late days are consumed, you'll receive no credit for late assignments. If you submit an assignment late, notify the TA by email.

### Programming Guidelines.
Assignments in this course will be completed in [Python 2.7](https://www.python.org/download/releases/2.7/).

Code style should follow the guidelines established in [PEP 8](http://legacy.python.org/dev/peps/pep-0008/) and [PEP 257](http://legacy.python.org/dev/peps/pep-0257/).

###### Note: the course logo image is copyright flickr user Dominic Alves, used under [Creative Commons](https://creativecommons.org/licenses/by/2.0/) license.
