Tasker Web App
================

Tasker is a web application for managing tasks. It allows users to register and log in, view, add, edit, and delete tasks, archive completed tasks, and export completed tasks to a Microsoft Word document.

Installation
------------

To install Tasker, follow these steps:

1. Clone the repository:
```bash
git clone https://github.com/cloverfield11/Task-Manager-Python
```
2. Use project directory:
```
cd Task-Manager-Python
```
3. Create a virtual environment:
```
python3 -m venv venv
```
4. Activate the virtual environment:
```bash
source venv/bin/activate
```
5. Install the required packages:
```
pip install -r requirements.txt
```
6. Run the application:
```bash
python3 main.py
```
The application will be available at `http://localhost:5000`.

Usage
-----

### User Authentication
#### WARNING!!! To keep records in a table use | LOGIN: admin | PASSWORD: admin |

To register, go to the `/register` page and enter a username and password. To log in, go to the `/login` page and enter your username and password.

### Task Management

To view the tasks, go to the `/index` page. The tasks are grouped into three categories: Current tasks, Additional tasks, and Completed tasks. The tasks are color-coded based on their priority: High (red), Medium (orange), and Low (green). The due date is formatted in the "DD month MMYY" format, where "DD" is the day of the month, "month" is the month name in Russian, and "MMYY" is the two-digit month and year.

To add a new task, go to the `/add_task` page and enter the task details. To edit an existing task, go to the `/task/<int:task_id>` page and click the "Edit" button. To delete a task, go to the `/task/<int:task_id>` page and click the "Delete" button.

### Task Archiving

To archive completed tasks, go to the `/archive_tasks` page and click the "Archive" button. The completed tasks will be moved to the `/archive_index` page.

### Task Export

To export completed tasks to a Microsoft Word document, go to the `/export_docx` page. The document will contain the task name, description, category, deadline, and comments.

Contributing
------------

If you want to contribute to Tasker, please follow these steps:

1. Fork the repository.
2. Create a new branch:
```bash
git checkout -b my-new-feature
```
3. Make changes and commit them:
```bash
git commit -am 'Add some feature'
```
4. Push to the branch:
```bash
git push origin my-new-feature
```
5. Submit a pull request.
