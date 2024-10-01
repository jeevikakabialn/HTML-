css
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Course Registration and Payment Form</title>
    <!-- Bootstrap 5 CDN -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        /* Form container styling */
        .form-container {
            max-width: 800px;
            margin: 50px auto;
            padding: 30px;
            background-color: #f9f9f9;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        /* Form heading */
        .form-heading {
            text-align: center;
            font-size: 28px;
            font-weight: bold;
            margin-bottom: 30px;
            color: #333;
        }

        /* Form control styling */
        .form-control {
            margin-bottom: 20px;
            padding: 10px;
            border-radius: 4px;
            border: 1px solid #ccc;
        }

        /* Label styling */
        .form-label {
            font-weight: 600;
            font-size: 16px;
            color: #555;
        }

        /* Select box styling */
        .form-select {
            margin-bottom: 20px;
            padding: 10px;
            border-radius: 4px;
            border: 1px solid #ccc;
        }

        /* Submit button styling */
        .btn-submit {
            background-color: #28a745;
            color: #fff;
            font-size: 18px;
            font-weight: 600;
            padding: 12px 25px;
            border-radius: 4px;
            border: none;
            transition: background-color 0.3s;
        }

        .btn-submit:hover {
            background-color: #218838;
        }

        /* Additional Comments Textarea */
        textarea {
            resize: vertical;
        }

        /* Custom Checkbox and Radio Styles */
        .custom-checkbox .custom-control-input:checked ~ .custom-control-label::before {
            background-color: #28a745;
            border-color: #28a745;
        }

        /* Spacing between form sections */
        .form-section {
            margin-bottom: 30px;
        }

        /* Responsive adjustments */
        @media (max-width: 768px) {
            .form-heading {
                font-size: 24px;
            }

            .btn-submit {
                width: 100%;
                font-size: 16px;
            }

            .form-container {
                padding: 20px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="form-container">
            <h2 class="form-heading">Course Registration and Payment Form</h2>
            <form>
                <!-- Student Name -->
                <div class="row mb-3">
                    <div class="col-md-4">
                        <label for="firstName" class="form-label">First Name</label>
                        <input type="text" class="form-control" id="firstName" placeholder="First Name">
                    </div>
                    <div class="col-md-4">
                        <label for="middleName" class="form-label">Middle Name</label>
                        <input type="text" class="form-control" id="middleName" placeholder="Middle Name">
                    </div>
                    <div class="col-md-4">
                        <label for="lastName" class="form-label">Last Name</label>
                        <input type="text" class="form-control" id="lastName" placeholder="Last Name">
                    </div>
                </div>

                <!-- Date of Birth -->
                <div class="row mb-3">
                    <div class="col-md-4">
                        <label for="birthMonth" class="form-label">Month</label>
                        <select id="birthMonth" class="form-select">
                            <option selected>Choose...</option>
                            <option>January</option>
                            <option>February</option>
                        </select>
                    </div>
                    <div class="col-md-4">
                        <label for="birthDay" class="form-label">Day</label>
                        <select id="birthDay" class="form-select">
                            <option selected>Choose...</option>
                            <option>1</option>
                            <option>2</option>
                        </select>
                    </div>
                    <div class="col-md-4">
                        <label for="birthYear" class="form-label">Year</label>
                        <select id="birthYear" class="form-select">
                            <option selected>Choose...</option>
                            <option>2000</option>
                            <option>2001</option>
                        </select>
                    </div>
                </div>

                <!-- Gender -->
                <div class="mb-3">
                    <label for="gender" class="form-label">Gender</label>
                    <select id="gender" class="form-select">
                        <option selected>Choose...</option>
                        <option>Male</option>
                        <option>Female</option>
                    </select>
                </div>

                <!-- Address -->
                <div class="mb-3">
                    <label for="address" class="form-label">Address</label>
                    <input type="text" class="form-control" id="address" placeholder="Street Address">
                    <input type="text" class="form-control mt-2" placeholder="Street Address Line 2">
                    <input type="text" class="form-control mt-2" placeholder="City">
                    <input type="text" class="form-control mt-2" placeholder="State/Province">
                    <input type="text" class="form-control mt-2" placeholder="Postal/Zip Code">
                </div>

                <!-- Email -->
                <div class="mb-3">
                    <label for="email" class="form-label">Student Email</label>
                    <input type="email" class="form-control" id="email" placeholder="example@example.com">
                </div>

                <!-- Mobile Number -->
                <div class="mb-3">
                    <label for="mobileNumber" class="form-label">Mobile Number</label>
                    <input type="text" class="form-control" id="mobileNumber" placeholder="(000) 000-0000">
                </div>

                <!-- Profession -->
                <div class="mb-3">
                    <label for="profession" class="form-label">Profession</label>
                    <input type="text" class="form-control" id="profession" placeholder="Profession">
                </div>

                <!-- Course Selection -->
                <div class="mb-3">
                    <label for="course" class="form-label">Select Course</label>
                    <select id="course" class="form-select">
                        <option selected>Choose...</option>
                        <option>Course 1</option>
                        <option>Course 2</option>
                    </select>
                </div>

                <!-- Additional Comments -->
                <div class="mb-3">
                    <label for="additionalComments" class="form-label">Additional Comments</label>
                    <textarea id="additionalComments" class="form-control" rows="4" placeholder="Enter any additional comments"></textarea>
                </div>

                <!-- Submit Button -->
                <div class="text-center">
                    <button type="submit" class="btn btn-submit">Submit</button>
                </div>
            </form>
        </div>
    </div>

    <!-- Bootstrap 5 JavaScript CDN -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>




<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Course Registration and Payment Form</title>
    <!-- Bootstrap 5 CDN -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        .form-heading {
            text-align: center;
            margin-bottom: 20px;
        }
        .form-control {
            margin-bottom: 15px;
        }
        .btn-submit {
            background-color: #28a745;
            color: white;
            font-size: 18px;
            padding: 10px 20px;
        }
        .form-container {
            max-width: 700px;
            margin: 0 auto;
            padding: 20px;
            border: 1px solid #ddd;
            border-radius: 10px;
        }
        .form-group label {
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="form-container">
            <h2 class="form-heading">Course Registration and Payment Form</h2>
            <form>
                <!-- Student Name -->
                <div class="row mb-3">
                    <div class="col-md-4">
                        <label for="firstName" class="form-label">First Name</label>
                        <input type="text" class="form-control" id="firstName" placeholder="First Name">
                    </div>
                    <div class="col-md-4">
                        <label for="middleName" class="form-label">Middle Name</label>
                        <input type="text" class="form-control" id="middleName" placeholder="Middle Name">
                    </div>
                    <div class="col-md-4">
                        <label for="lastName" class="form-label">Last Name</label>
                        <input type="text" class="form-control" id="lastName" placeholder="Last Name">
                    </div>
                </div>

                <!-- Date of Birth -->
                <div class="row mb-3">
                    <div class="col-md-4">
                        <label for="birthMonth" class="form-label">Month</label>
                        <select id="birthMonth" class="form-select">
                            <option selected>Choose...</option>
                            <!-- Add more months -->
                            <option>January</option>
                            <option>February</option>
                        </select>
                    </div>
                    <div class="col-md-4">
                        <label for="birthDay" class="form-label">Day</label>
                        <select id="birthDay" class="form-select">
                            <option selected>Choose...</option>
                            <!-- Add days 1-31 -->
                            <option>1</option>
                            <option>2</option>
                        </select>
                    </div>
                    <div class="col-md-4">
                        <label for="birthYear" class="form-label">Year</label>
                        <select id="birthYear" class="form-select">
                            <option selected>Choose...</option>
                            <!-- Add years -->
                            <option>2000</option>
                            <option>2001</option>
                        </select>
                    </div>
                </div>

                <!-- Gender -->
                <div class="mb-3">
                    <label for="gender" class="form-label">Gender</label>
                    <select id="gender" class="form-select">
                        <option selected>Choose...</option>
                        <option>Male</option>
                        <option>Female</option>
                    </select>
                </div>

                <!-- Address -->
                <div class="mb-3">
                    <label for="address" class="form-label">Address</label>
                    <input type="text" class="form-control" id="address" placeholder="Street Address">
                    <input type="text" class="form-control mt-2" placeholder="Street Address Line 2">
                    <input type="text" class="form-control mt-2" placeholder="City">
                    <input type="text" class="form-control mt-2" placeholder="State/Province">
                    <input type="text" class="form-control mt-2" placeholder="Postal/Zip Code">
                </div>

                <!-- Email -->
                <div class="mb-3">
                    <label for="email" class="form-label">Student Email</label>
                    <input type="email" class="form-control" id="email" placeholder="example@example.com">
                </div>

                <!-- Mobile Number -->
                <div class="mb-3">
                    <label for="mobileNumber" class="form-label">Mobile Number</label>
                    <input type="text" class="form-control" id="mobileNumber" placeholder="(000) 000-0000">
                </div>

                <!-- Profession -->
                <div class="mb-3">
                    <label for="profession" class="form-label">Profession</label>
                    <input type="text" class="form-control" id="profession" placeholder="Profession">
                </div>

                <!-- Course Selection -->
                <div class="mb-3">
                    <label for="course" class="form-label">Select Course</label>
                    <select id="course" class="form-select">
                        <option selected>Choose...</option>
                        <!-- Add more courses -->
                        <option>Course 1</option>
                        <option>Course 2</option>
                    </select>
                </div>

                <!-- Additional Comments -->
                <div class="mb-3">
                    <label for="additionalComments" class="form-label">Additional Comments</label>
                    <textarea id="additionalComments" class="form-control" rows="4" placeholder="Enter any additional comments"></textarea>
                </div>

                <!-- Submit Button -->
                <div class="text-center">
                    <button type="submit" class="btn btn-submit">Submit</button>
                </div>
            </form>
        </div>
    </div>

    <!-- Bootstrap 5 JavaScript CDN -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
