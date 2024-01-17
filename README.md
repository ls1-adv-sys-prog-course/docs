# Practical course: Advanced Systems Programming -- SoSe 2024

## Chair website

- The practical course is organized by the [Chair of Computer Systems](https://dse.in.tum.de/) at TU Munich.

## Course Information
- Language: English
- Type: Practical training
- Module: IN0012, IN2106, IN2128
- SWS: 6
- ECTS Credits: 10
- Prerequisites:
    - *The students must successfully finish the following course beforehand.*
        - Practical Lab: Systems Programming (2023-)
        - Practical Lab: Advanced Systems Programming in C/Rust (offered in 2021-2023)
    - Preferred knowledge or equivalent to the lectures
        - Fundamentals of Programming (IN0002)
        - Introduction to Computer Architecture (IN0004)
        - Basic Principles: Operating Systems and System Software (IN0009)
- Course Material:
    - The Linux Programming Interface – Michael Kerrisk
    - Linux System Programming – Robert Love
- TUM Online:
    - You must register for this course in TUM Online before the course starts
- Student note:
    - Compulsory enrollment after two weeks of the matching outcome; students who fail to de-register in this period will be registered for the exam
    - This course differs from the "Practical Lab: Advanced Systems Programming in C/Rust" offered in 2021-2023. That course is now called "Practical Lab: Systems Programming." This course covers more advanced topics than the "Practical Lab: Systems Programming".

## Course Details
This course covers some of the advanced topics in system programming. More specifically, we will cover the following topics through a set of programming assignments over the semester:

- Containers: How to use Linux's namespace and cgroup to realize os-level virtualization (aka containers).
- Unikernels How to write and extend application-specialized operating systems with the Unikraft unikernel.
- Hypervisors: How to create hypervisors with hardware-assisted virtualization features to run virtual machines using Linux's KVM.
- Hardware Acceleration: How to modify an application to take advantage of a custom accelerator, implementing necessary software components to interact with the hardware and optimizing the interface between software and hardware.

This course consists of programming assignments that will help students dig deeper into the concepts and get familiar with them. The students will be required to perform tasks within a time frame (around 2-3 weeks, depending on the task) and submit their work in the online evaluation system. The submitted workpieces will then be evaluated, and a grade will be calculated based on that. There is a weekly Q&A meeting where we answer students' questions and discuss the specific goal of each assignment. We also have an online discussion place.

## Objectives
- Learn advanced topics related to computer systems
- Be able to write low-level code to manage complex systems

## Meeting place

- Preliminary meeting: Feb 1st (Thu), 2024 10:00 AM CET online (zoom)
    - [Zoom link](https://tum-conf.zoom-x.de/j/62687139904?pwd=SFNmQUIvT0tRaHlDaVYrN3l5bzJVQT09)
    - Meeting ID: 626 8713 9904, Passcode: 0
- Q&A session: Weekly on Thursday from 03:00 PM to 04:00 PM CET
    - Place: TBA
    - If the day is a holiday, we will have the session on the previous day.

## Tasks

Please refer to the respective task repositories (that are released on the published date) for detail.
The schedule may change. **All deadlines are at 15:00 (CEST).**


| Task            | Published on | Deadline   | Points | Slide | Video |
|-----------------|--------------|------------|--------|-------|-------|
| Containers      | 2024-04-15   | 2024-05-06 | 40     |       |       |
| Unikernels      | 2024-05-06   | 2024-05-27 | 40     |       |       |
| Hypervisors     | 2024-05-27   | 2024-06-17 | 40     |       |       |
| HW Accelaration | 2024-06-17   | 2024-07-08 | 40     |       |       |


Note that
- 100% points lost if private tests detect cheating or we find a solution tries to game the system (modifying test scripts, etc.)
- 50% points lost if normal private tests fail


## Allowed Libraries

In general, only standard libraries can be used. In addition to this, the following libraries are available for use.

- Rust: [libc](https://crates.io/crates/libc), [nix](https://crates.io/crates/nix)
- C++: [{fmt}](https://fmt.dev/latest/index.html), [range-v3](https://github.com/ericniebler/range-v3)
- General argument parsing libraries, such as [clap](https://crates.io/crates/clap)
- General error handling libraries, such as [anyhow](https://docs.rs/anyhow/latest/anyhow/)

Depending on the task, the use of additional libraries may be allowed or the use of libraries (including standard libraries) may be restricted. Please refer to the task description for details.

For a reference of the standard library, check out:
- [cppreference](https://en.cppreference.com/w/) for C/C++
- [std](https://doc.rust-lang.org/std/) for rust

## Environment

All executables must run on Linux, x86_64. Therefore, we strongly recommend having a local Linux x86_64 environment for development.
Note that some tasks involve loading kernel modules and configuring kernel parameters, including cgroups, and some operations are not allowed in some container (docker) environments.
Each task gives more details information on runnable environments.

Note that only the test results on CI count toward grading.

## Grades

Grades are computed as follows:

|From  |   To    | Grade    | Interval |
|------|---------|----------|----------|
|0     |   80    | 5        | 80       |
|81    |   86    | 4.7      |  5       |
|87    |   92    | 4.3      |  5       |
|93    |   98    | 4        |  5       |
|99    |  104    | 3.7      |  5       |
|105   |  110    | 3.3      |  5       |
|111   |  116    | 3        |  5       |
|117   |  124    | 2.7      |  7       |
|125   |  132    | 2.3      |  7       |
|133   |  140    | 2        |  7       |
|141   |  148    | 1.7      |  7       |
|149   |  156    | 1.3      |  7       |
|157   |  160    | 1        |  3       |

## Slack workspace

We will use Slack for all communication. Please enroll in our Slack workspace using your official TUM email address.

- **Slack workspace:** https://ls1-courses-tum.slack.com
- **Slack channel:** #ss-24-adv-sys-prog

## Contact

We *strongly* prefer Slack for all communications. For any further questions/comments, please contact the course organizer(s):

- [Dr. Masanori Misono](https://mmisono.github.io/)
- [Prof. Bhatotia](https://dse.in.tum.de/bhatotia/)
