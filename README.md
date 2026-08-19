# Health-care
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>BloodConnect - Blood Donation</title>

    <style>
        /* ==============================
           GLOBAL STYLES
        =============

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #050505;
            color: #ffffff;
            line-height: 1.6;
        }

        /* ==============================
           HEADER
        ============================== */

        header {
            background: linear-gradient(135deg, #000000, #062526);
            text-align: center;
            padding: 45px 20px 30px;
            border-bottom: 2px solid #ff00c8;
            box-shadow: 0 0 25px #ff008c6b;
        }

        header h1 {
            color: #00ffff;
            font-size: 44px;
            margin-bottom: 10px;
            text-shadow: 0 0 15px rgba(0, 255, 255, 0.6);
        }

        header p {
            color: #c9ffff;
            font-size: 18px;
            margin-bottom: 25px;
        }

        /* ==============================
           NAVIGATION
        ============================== */

        nav {
            margin-top: 20px;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            display: inline-block;
            margin: 5px;
            padding: 9px 14px;
            border-radius: 7px;
            transition: 0.3s ease;
        }

        nav a:hover {
            background: #00ffff;
            color: #000000;
            box-shadow: 0 0 15px #00ffff;
        }

        /* ==============================
           HORIZONTAL LINE
        ============================== */

        hr {
            border: none;
            height: 1px;
            background: linear-gradient(
                to right,
                transparent,
                #00ffff,
                transparent
            );
        }

        /* ==============================
           SECTIONS
        ============================== */

        section {
            max-width: 1000px;
            margin: 35px auto;
            padding: 35px;
            background: #101010;
            border: 1px solid #008b8b;
            border-radius: 15px;
            box-shadow: 0 0 20px rgba(0, 255, 255, 0.08);
        }

        section:hover {
            box-shadow: 0 0 30px rgba(0, 255, 255, 0.15);
        }

        section h2 {
            color: #00ffff;
            font-size: 29px;
            margin-bottom: 18px;
            border-left: 5px solid #00ffff;
            padding-left: 12px;
        }

        section h3 {
            color: #66ffff;
            margin-top: 20px;
            margin-bottom: 8px;
        }

        section p {
            color: #dddddd;
            margin-bottom: 15px;
        }

        /* ==============================
           HOME SECTION
        ============================== */

        #home {
            text-align: center;
            background: linear-gradient(
                145deg,
                #101010,
                #062122
            );
        }

        #home h2 {
            border-left: none;
            padding-left: 0;
        }

        #home h3 {
            font-size: 22px;
            color: #00ffff;
            margin-top: 25px;
        }

        /* ==============================
           BUTTONS
        ============================== */

        button {
            background: #00ffff;
            color: #000000;
            border: 2px solid #00ffff;
            padding: 12px 24px;
            margin: 8px 6px 8px 0;
            border-radius: 7px;
            font-size: 15px;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        button:hover {
            background: #000000;
            color: #00ffff;
            box-shadow: 0 0 18px #00ffff;
            transform: translateY(-2px);
        }

        /* ==============================
           FORMS
        ============================== */

        form {
            margin-top: 20px;
        }

        label {
            display: inline-block;
            color: #00ffff;
            font-weight: bold;
            margin-bottom: 6px;
        }

        input,
        select,
        textarea {
            width: 100%;
            max-width: 650px;
            padding: 12px 14px;
            background: #050505;
            color: white;
            border: 1px solid #008b8b;
            border-radius: 7px;
            font-size: 15px;
            outline: none;
            transition: 0.3s ease;
        }

        input:focus,
        select:focus,
        textarea:focus {
            border-color: #00ffff;
            box-shadow: 0 0 12px rgba(0, 255, 255, 0.4);
        }

        textarea {
            resize: vertical;
        }

        select option {
            background: #000000;
            color: white;
        }

        input::placeholder,
        textarea::placeholder {
            color: #777777;
        }

        /* ==============================
           SPECIAL SECTIONS
        ============================== */

        #request {
            border-color: #00ffff;
        }

        #donate {
            border-color: #00cccc;
        }

        #find {
            border-color: #00ffff;
        }

        #about {
            background: #0b0b0b;
        }

        /* ==============================
           HOW IT WORKS
        ============================== */

        #how-it-works {
            background: linear-gradient(
                145deg,
                #101010,
                #071b1c
            );
        }

        .steps {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 15px;
            margin-top: 25px;
        }

        .step {
            background: #050505;
            border: 1px solid #008b8b;
            border-radius: 10px;
            padding: 20px;
            text-align: center;
            transition: 0.3s ease;
        }

        .step:hover {
            border-color: #00ffff;
            box-shadow: 0 0 15px rgba(0, 255, 255, 0.3);
            transform: translateY(-5px);
        }

        .step h3 {
            color: #00ffff;
            margin-bottom: 10px;
        }

        .step p {
            font-size: 14px;
        }

        /* ==============================
           FOOTER
        ============================== */

        footer {
            text-align: center;
            background: #000000;
            color: #00ffff;
            padding: 25px 15px;
            margin-top: 40px;
            border-top: 2px solid #00ffff;
            box-shadow: 0 -5px 20px rgba(0, 255, 255, 0.1);
        }

        footer p {6
            margin: 0;
        }

        /* ==============================
           RESPONSIVE DESIGN
        ============================== */

        @media (max-width: 768px) {

            header h1 {
                font-size: 34px;
            }

            header p {
                font-size: 16px;
            }

            nav a {
                font-size: 14px;
                padding: 7px 9px;
            }

            section {
                margin: 20px 12px;
                padding: 25px;
            }

            section h2 {
                font-size: 24px;
            }

            input,
            select,
            textarea {
                max-width: 100%;
            }

            .steps {
                grid-template-columns: 1fr 1fr;
            }

            button {
                width: 100%;
                margin-right: 0;
            }
        }

        @media (max-width: 480px) {

            header {
                padding: 30px 15px;
            }

            header h1 {
                font-size: 28px;
            }

            header p {
                font-size: 14px;
            }

            nav a {
                display: block;
                margin: 6px 0;
            }

            section {
                padding: 18px;
            }

            section h2 {
                font-size: 21px;
            }

            .steps {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>

<body>

    <!-- ==============================
         HEADER
    ============================== -->

    <header>

        <h1>🩸 BloodConnect</h1>

        <p>
            One Donation. One Life. One Connection.
        </p>

        <nav>
            <a href="#home">Home</a>
            <a href="#request">Need Blood</a>
            <a href="#donate">Donate Blood</a>
            <a href="#find">Find Blood</a>
            <a href="#how-it-works">How It Works</a>
            <a href="#about">About Us</a>
        </nav>

    </header>


    <hr>


    <!-- ==============================
         HOME
    ============================== -->

    <section id="home">

        <h2>Welcome to BloodConnect</h2>

        <p>
            BloodConnect helps people find blood donors during emergencies
            and allows willing donors to register for blood donation.
        </p>

        <h3>🚨 Need Blood Urgently?</h3>

        <p>
            Submit your blood requirement and find matching blood donors
            according to blood group and location.
        </p>

        <a href="#request">
            <button type="button">Request Blood</button>
        </a>

        <a href="#donate">
            <button type="button">❤️ Become a Donor</button>
        </a>

    </section>


    <hr>


    <!-- ==============================
         EMERGENCY BLOOD REQUEST
    ============================== -->

    <section id="request">

        <h2>🚨 Emergency Blood Request</h2>

        <form>

            <label for="patient">Patient Name:</label>
            <br>

            <input
                type="text"
                id="patient"
                name="patient"
                placeholder="Enter patient name"
                required
            >

            <br><br>


            <label for="required-blood">
                Blood Group Required:
            </label>
            <br>

            <select id="required-blood" name="bloodgroup" required>

                <option value="">
                    Select Blood Group
                </option>

                <option>A+</option>
                <option>A-</option>
                <option>B+</option>
                <option>B-</option>
                <option>AB+</option>
                <option>AB-</option>
                <option>O+</option>
                <option>O-</option>

            </select>

            <br><br>


            <label for="units">Units Required:</label>
            <br>

            <input
                type="number"
                id="units"
                name="units"
                min="1"
                placeholder="Enter number of units"
                required
            >

            <br><br>


            <label for="hospital">Hospital Name:</label>
            <br>

            <input
                type="text"
                id="hospital"
                name="hospital"
                placeholder="Enter hospital name"
                required
            >

            <br><br>


            <label for="address">Hospital Address:</label>
            <br>

            <textarea
                id="address"
                name="address"
                rows="3"
                placeholder="Enter complete hospital address"
                required
            ></textarea>

            <br><br>


            <label for="city">City:</label>
            <br>

            <input
                type="text"
                id="city"
                name="city"
                placeholder="Enter city"
                required
            >

            <br><br>


            <label for="required-date">
                Required Date:
            </label>
            <br>

            <input
                type="date"
                id="required-date"
                name="required-date"
                required
            >

            <br><br>


            <label for="required-time">
                Required Time:
            </label>
            <br>

            <input
                type="time"
                id="required-time"
                name="required-time"
                required
            >

            <br><br>


            <label for="contact">
                Contact Number:
            </label>
            <br>

            <input
                type="tel"
                id="contact"
                name="contact"
                placeholder="Enter contact number"
                required
            >

            <br><br>


            <label for="emergency">
                Emergency Level:
            </label>
            <br>

            <select id="emergency" name="emergency">

                <option>Normal</option>
                <option>Urgent</option>
                <option>Critical</option>

            </select>

            <br><br>


            <label for="additional">
                Additional Information:
            </label>
            <br>

            <textarea
                id="additional"
                name="additional"
                rows="4"
                placeholder="Enter any additional information"
            ></textarea>

            <br><br>


            <button type="submit">
                🚨 Submit Blood Request
            </button>

        </form>

    </section>


    <hr>


    <!-- ==============================
         DONOR REGISTRATION
    ============================== -->

    <section id="donate">

        <h2>❤️ Become a Blood Donor</h2>

        <p>
            Register yourself as a donor and help someone in need.
        </p>

        <form>

            <label for="donor-name">
                Full Name:
            </label>
            <br>

            <input
                type="text"
                id="donor-name"
                name="donor-name"
                placeholder="Enter your full name"
                required
            >

            <br><br>


            <label for="age">Age:</label>
            <br>

            <input
                type="number"
                id="age"
                name="age"
                min="18"
                placeholder="Enter your age"
                required
            >

            <br><br>


            <label for="donor-blood">
                Blood Group:
            </label>
            <br>

            <select
                id="donor-blood"
                name="donor-blood"
                required
            >

                <option value="">
                    Select Blood Group
                </option>

                <option>A+</option>
                <option>A-</option>
                <option>B+</option>
                <option>B-</option>
                <option>AB+</option>
                <option>AB-</option>
                <option>O+</option>
                <option>O-</option>

            </select>

            <br><br>


            <label for="donor-city">
                City:
            </label>
            <br>

            <input
                type="text"
                id="donor-city"
                name="donor-city"
                placeholder="Enter city"
                required
            >

            <br><br>


            <label for="area">
                Area:
            </label>
            <br>

            <input
                type="text"
                id="area"
                name="area"
                placeholder="Enter area"
                required
            >

            <br><br>


            <label for="phone">
                Phone Number:
            </label>
            <br>

            <input
                type="tel"
                id="phone"
                name="phone"
                placeholder="Enter phone number"
                required
            >

            <br><br>


            <label for="email">
                Email:
            </label>
            <br>

            <input
                type="email"
                id="email"
                name="email"
                placeholder="Enter email address"
            >

            <br><br>


            <label for="last-donation">
                Last Donation Date:
            </label>
            <br>

            <input
                type="date"
                id="last-donation"
                name="last-donation"
            >

            <br><br>


            <label for="preferred-date">
                Preferred Donation Date:
            </label>
            <br>

            <input
                type="date"
                id="preferred-date"
                name="preferred-date"
                required
            >

            <br><br>


            <label for="preferred-time">
                Preferred Time:
            </label>
            <br>

            <input
                type="time"
                id="preferred-time"
                name="preferred-time"
                required
            >

            <br><br>


            <button type="submit">
                ❤️ Register as Donor
            </button>

        </form>

    </section>


    <hr>


    <!-- ==============================
         FIND BLOOD
    ============================== -->

    <section id="find">

        <h2>🔎 Find Blood</h2>

        <form>

            <label for="find-blood">
                Blood Group:
            </label>
            <br>

            <select
                id="find-blood"
                name="find-blood"
                required
            >

                <option value="">
                    Select Blood Group
                </option>

                <option>A+</option>
                <option>A-</option>
                <option>B+</option>
                <option>B-</option>
                <option>AB+</option>
                <option>AB-</option>
                <option>O+</option>
                <option>O-</option>

            </select>

            <br><br>


            <label for="find-city">
                City:
            </label>
            <br>

            <input
                type="text"
                id="find-city"
                name="find-city"
                placeholder="Enter city"
            >

            <br><br>


            <label for="find-area">
                Area:
            </label>
            <br>

            <input
                type="text"
                id="find-area"
                name="find-area"
                placeholder="Enter area"
            >

            <br><br>


            <label for="find-units">
                Units Required:
            </label>
            <br>

            <input
                type="number"
                id="find-units"
                name="find-units"
                min="1"
                placeholder="Enter units required"
            >

            <br><br>


            <button type="submit">
                🔎 Search Blood
            </button>

        </form>

    </section>


    <hr>


    <!-- ==============================
         HOW IT WORKS
    ============================== -->

    <section id="how-it-works">

        <h2>⚙️ How BloodConnect Works</h2>

        <div class="steps">

            <div class="step">

                <h3>1️⃣ Request</h3>

                <p>
                    Enter the patient's blood requirement,
                    hospital and location.
                </p>

            </div>


            <div class="step">

                <h3>2️⃣ Match</h3>

                <p>
                    Find available donors with the required
                    blood group.
                </p>

            </div>


            <div class="step">

                <h3>3️⃣ Connect</h3>

                <p>
                    Connect the blood seeker with a matching
                    donor.
                </p>

            </div>


            <div class="step">

                <h3>4️⃣ Donate</h3>

                <p>
                    Donors visit the selected donation center
                    at the scheduled time.
                </p>

            </div>

        </div>

    </section>


    <hr>


    <!-- ==============================
         ABOUT US
    ============================== -->

    <section id="about">

        <h2>ℹ️ About BloodConnect</h2>

        <p>
            BloodConnect is a student project designed to make
            blood donation and emergency blood searching easier
            and faster.
        </p>

        <p>
            This platform is intended to connect donors and people
            looking for blood. Actual blood donation and eligibility
            must always be confirmed by qualified medical
            professionals or authorized blood banks.
        </p>

    </section>


    <!-- ==============================
         FOOTER
    ============================== -->

    <footer>

        <p>
            © 2026 BloodConnect | Save Lives, Donate Blood ❤️
        </p>

    </footer>

</body>

</html>
