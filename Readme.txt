Policy Management System

Description:
The Policy Management System is designed for an insurance company to manage policyholders, products, and payments. It allows policy managers to register new policyholders, suspend or reactivate them, manage insurance products, and process payments. The system demonstrates basic functionalities such as registering policyholders for products, processing payments, applying penalties, and sending payment reminders.
This project is built in Python, with separate class files for each functional area (policyholders, products, and payments). The main script demonstrates how these components work together.

Project Structure:
•	policyholder.py: Contains the Policyholder class which manages policyholder registration, suspension, reactivation, and displaying policyholder details.
•	product.py: Contains the Product class which handles creation, updating, and suspending or reactivating products.
•	payment.py: Contains the Payment class responsible for processing payments, sending reminders, and applying penalties.
•	main.py: Demonstrates how to use the classes by creating two policyholders, registering them for products, processing payments, and displaying their details.
•	README.txt: This file, providing a detailed description of the project, its structure, how to run it, and other important details.
________________________________________
Features:
•	Policyholder Management:
	o	Register new policyholders.
	o	Suspend and reactivate policyholders.
	o	Display policyholder details including their registered products.
•	Product Management:
	o	Create new insurance products.
	o	Update product names.
	o	Suspend or reactivate products.
•	Payment Management:
	o	Process payments for policyholders.
	o	Send payment reminders.
	o	Apply penalties for late payments.
	o	Display payment details.
Requirements:
•	Python 3.x installed on your machine.
•	Visual Studio with the Python plugin installed.

How to Run the Project in Visual Studio:
1.	Clone the Repository: Download or clone the project to your local machine.
2.	Open Visual Studio: Launch Visual Studio and ensure the Python plugin is installed.
3.	Create a New Python Project:
	o	Go to File > New > Project.
	o	Choose Python Application from the project types.
	o	Name your project and select the location where you want to save it.
4.	Add Project Files:
	o	Right-click the project in the Solution Explorer.
	o	Select Add > New Item and add Python files for each of the classes (policyholder.py, product.py, payment.py) and the main script (main.py).
	o	Copy the respective code into each of these files.
5.	Run the Main Script:
	o	Make sure the main.py file is the startup file (right-click on main.py in Solution Explorer and select Set as Startup File).
	o	Press F5 or click Start to run the project.
6.	Output: The output will be displayed in the Output Window or Terminal at the bottom of Visual Studio, showing the details of the policyholders and their payments.


File Descriptions:
1.	policyholder.py:
	o	Class: Policyholder
	o	Attributes:
			policyholder_id: The unique identifier for the policyholder.
			name: The policyholder's name.
			status: The current status of the policyholder (Active/Suspended).
			products: List of products the policyholder has registered for.

o	Methods:
			register(product): Adds a product to the policyholder’s account.
			suspend(): Suspends the policyholder's account.
			reactivate(): Reactivates the policyholder's account.
			display_details(): Displays the policyholder's details.

2.	product.py:
	o	Class: Product
	o	Attributes:
			product_id: Unique identifier for the product.
			name: Name of the product.
			status: Current status of the product (Available/Suspended).
	o	Methods:
			update_product(new_name): Updates the product's name.
			suspend_product(): Suspends the product from being available.
			reactivate_product(): Reactivates the product.
			display_product(): Displays product details.
3.	payment.py:
	o	Class: Payment
	o	Attributes:
			policyholder: The policyholder making the payment.
			amount: The amount to be paid.
			status: The payment status (Pending/Paid).
	o	Methods:
			process_payment(): Marks the payment as paid.
			send_reminder(): Sends a payment reminder.
			apply_penalty(penalty_amount): Applies a penalty to the payment.
			display_payment_details(): Displays the payment details.
4.	main.py:
	o	Demonstrates the functionality by creating instances of policyholders, products, and payments.
	o	Processes payments for two policyholders and displays their account and payment details.



