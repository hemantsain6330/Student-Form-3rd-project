//Sourse code.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modern Student Registration Portal</title>
    <link rel="stylesheet" href="style.css">
    <!-- FontAwesome for cool icons --/>
</head>
<body>
    <div class="container">
        <div class="form-header">
            <h2><i class="fas fa-graduation-cap"></i> Student Portal</h2>
            <p>Join our learning community today</p>
        </div>
        
        <form id="studentForm">
            <div class="input-group">
                <label for="fullName">Full Name</label>
                <div class="input-field">
                    <i class="fas fa-user"></i>
                    <input type="text" id="fullName" placeholder="Enter full name" required>
                </div>
            </div>

            <div class="input-group">
                <label for="email">Email Address</label>
                <div class="input-field">
                    <i class="fas fa-envelope"></i>
                    <input type="email" id="email" placeholder="example@email.com" required>
                </div>
            </div>

            <div class="row">
                <div class="input-group">
                    <label for="phone">Phone Number</label>
                    <div class="input-field">
                        <i class="fas fa-phone"></i>
                        <input type="tel" id="phone" placeholder="10-digit number" required>
                    </div>
                </div>
                <div class="input-group">
                    <label for="dob">Date of Birth</label>
                    <div class="input-field">
                        <i class="fas fa-calendar-alt"></i>
                        <input type="date" id="dob" required>
                    </div>
                </div>
            </div>

            <!-- Course Selection Dropdown -->
            <div class="input-group">
                <label for="course">Select Course</label>
                <div class="input-field">
                    <i class="fas fa-book"></i>
                    <select id="course" required>
                        <option value="" disabled selected>Choose your course</option>
                        <option value="BCA">Bachelor of Computer Applications (BCA)</option>
                        <option value="BBA">Bachelor of Business Administration (BBA)</option>
                        <option value="B.Tech">Bachelor of Technology (B.Tech)</option>
                        <option value="LLB">Bachelor of Laws (LLB)</option>
                        <option value="Bachelor of Arts">Bachelor of Arts (BA)</option>
                    </select>
                </div>
            </div>

            <!-- University/College Selection Dropdown -->
            <div class="input-group">
                <label for="university">Select University / College</label>
                <div class="input-field">
                    <i class="fas fa-university"></i>
                    <select id="university" required>
                        <option value="" disabled selected>Choose your institution</option>
                        <option value="Lucknow University">Lucknow University</option>
                        <option value="Raja Mahendra Pratap Singh University">Raja Mahendra Pratap Singh State University</option>
                        <option value="Aligarh Muslim University (AMU)">Aligarh Muslim University (AMU)</option>
                        <option value="Chaudhary Harchana Singh Group of College (CHSGC)">Chaudhary Harchana Singh Group of College (CHSGC)</option>
                    </select>
                </div>
            </div>

            <button type="submit" class="btn-submit">
                Register Student <i class="fas fa-arrow-right"></i>
            </button>
        </form>
    </div>

    <!-- Success Modal Popup -->
    <div class="modal" id="successModal">
        <div class="modal-content">
            <i class="fas fa-check-circle success-icon"></i>
            <h3>Registration Successful!</h3>
            <!-- Dynamic confirmation message goes here via JS -->
            <p id="successMessage">Your profile has been created successfully.</p>
            <button onclick="closeModal()" class="btn-close">Awesome</button>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
