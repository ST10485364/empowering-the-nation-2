#ST10485364
#ST10481692
The app is a dynamic web-based platform designed to assist users in calculating the total fee for a selected course based on the number of participants. 
Upon accessing the course detail page, the app retrieves the course information—such as the course name, description, and base price—from a predefined dataset using JavaScript.
This data is then displayed on the page, providing users with an overview of the course. To calculate the total fee, users input the number of students into
a designated field and click the 'Calculate' button. The app then multiplies the base price by the number of students and presents the total fee in a user-friendly format.
This interactive feature ensures that users can easily determine the cost of enrolling multiple participants in a course, enhancing the overall user experience.






empowering-the-nation/
│
├── index.html
├── courses.html
├── courses-detail.html
├── contact.html
├── styles.css
└── common.js



INDEX-<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Empowering the Nation — Skills & Courses</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="header">
    <div class="container nav">
      <div class="brand">
        <img src="logo.jpg" alt="logo" />
        <div>
          <strong>Empowering the Nation</strong>
          <div class="small">Skills & training for domestic workers and gardeners</div>
        </div>
      </div>
      <nav>
        <a href="index.html">Home</a>
        <a href="courses.html">Courses</a>
        <a href="contact.html">Contact</a>
        <a class="btn" href="courses.html">Browse Courses</a>
      </nav>
    </div>
  </header>

  <main class="container">
    <section class="hero">
      <div class="left">
        <h1>Practical, affordable training for everyday skills</h1>
        <p>Short, hands-on courses that prepare learners for household and gardening work — with certificates and group discounts.</p>
        <div class="cta">
          <a class="btn" href="courses.html">See courses</a>
          <a href="contact.html">Get in touch</a>
        </div>
      </div>

      <div class="right card" style="width:320px">
        <h3 style="margin-top:0">Quick fee calculator</h3>
        <div class="small">Enter number of participants to estimate total cost</div>
        <div style="margin-top:12px">
          <select id="courseSelect" class="input"></select>
          <div style="height:8px"></div>
          <input id="participants" class="input" type="number" placeholder="Number of participants" min="1" value="1" />
          <div style="height:12px"></div>
          <button class="btn" id="calcBtn">Calculate</button>
          <div id="calcResult" style="margin-top:12px;font-weight:600"></div>
        </div>
      </div>
    </section>

    <section>
      <h2>Popular courses</h2>
      <div class="grid" id="coursesGrid"></div>
    </section>
  </main>

  <footer class="container footer">
    <div style="display:flex;justify-content:space-between;align-items:center">
      <div>© 2025 Empowering the Nation</div>
      <div><a href="#">Privacy</a> • <a href="#">Terms</a></div>
    </div>
  </footer>

  <script src="common.js"></script>
</body>
</html>




Courses- <!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Courses — Empowering the Nation</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="header">
    <div class="container nav">
      <div class="brand">
        <img src="logo.jpg" alt="logo" />
        <div><strong>Empowering the Nation</strong></div>
      </div>
      <nav>
        <a href="index.html">Home</a>
        <a href="courses.html">Courses</a>
        <a href="contact.html">Contact</a>
      </nav>
    </div>
  </header>

  <main class="container">
    <h1>All Courses</h1>
    <p class="small">Click a course to view details and calculate fees.</p>
    <div class="grid" id="coursesGridAll"></div>
  </main>

  <footer class="container footer">© 2025 Empowering the Nation</footer>
  <script src="common.js"></script>
</body>
</html>




courses detail- <!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Course Details</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="header">
    <div class="container nav">
      <div class="brand">
        <img src="logo.jpg" alt="logo" />
        <div><strong>Empowering the Nation</strong></div>
      </div>
      <nav>
        <a href="index.html">Home</a>
        <a href="courses.html">Courses</a>
        <a href="contact.html">Contact</a>
      </nav>
    </div>
  </header>

  <main class="container">
    <a href="courses.html">← Back to courses</a>
    <div class="card" style="margin-top:16px">
      <h2 id="courseName">Course name</h2>
      <p id="courseDesc" class="course-desc">Course description</p>
      <div class="small">Price per participant: <span id="coursePrice">R0</span></div>

      <hr style="margin:18px 0" />
      <h3>Calculate total fee</h3>
      <div class="form-row" style="margin-top:8px">
        <input id="numStudents" class="input" type="number" min="1" value="1" />
        <button id="calcDetail" class="btn">Calculate</button>
      </div>
      <div id="detailResult" style="margin-top:12px;font-weight:600"></div>
    </div>
  </main>

  <footer class="container footer">© 2025 Empowering the Nation</footer>
  <script src="common.js"></script>
</body>
</html>







contact-<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Contact — Empowering the Nation</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="header">
    <div class="container nav">
      <div class="brand">
        <img src="logo.jpg" alt="logo" />
        <div><strong>Empowering the Nation</strong></div>
      </div>
      <nav>
        <a href="index.html">Home</a>
        <a href="courses.html">Courses</a>
      </nav>
    </div>
  </header>

  <main class="container">
    <h1>Contact Us</h1>
    <p class="small">Fill in the form and we'll get back to you within 2 working days.</p>
    <div class="card" style="max-width:640px">
      <label class="small">Your name</label>
      <input id="name" class="input" placeholder="Your full name" />
      <label class="small">Email</label>
      <input id="email" class="input" type="email" placeholder="you@example.com" />
      <label class="small">Message</label>
      <textarea id="message" class="input" rows="5" placeholder="How can we help?"></textarea>
      <div style="height:12px"></div>
      <button id="sendBtn" class="btn">Send message</button>
      <div id="sendResult" style="margin-top:10px" class="small"></div>
    </div>
  </main>

  <footer class="container footer">© 2025 Empowering the Nation</footer>
  <script src="common.js"></script>
</body>
</html>






styles- :root {
  --accent: #0d6efd;
  --muted: #6b7280;
  --bg: #f8fafc;
  --card: #ffffff;
  --radius: 12px;
  --maxw: 1100px;
}
* { box-sizing: border-box; }
html, body { height: 100%; }
body {
  margin: 0;
  font-family: Inter, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial;
  background: var(--bg);
  color: #111827;
  line-height: 1.45;
}
.container { max-width: var(--maxw); margin: 0 auto; padding: 24px; }
.header { background: linear-gradient(90deg, rgba(13,110,253,0.06), transparent); }
.nav { display: flex; align-items: center; justify-content: space-between; padding: 14px 0; }
.brand { display: flex; gap: 12px; align-items: center; }
.brand img { height: 48px; border-radius: 8px; }
.nav a { color: #0f172a; text-decoration: none; margin-left: 16px; font-weight: 600; }
.btn {
  background: var(--accent); color: white; padding: 10px 14px;
  border-radius: 10px; text-decoration: none; display: inline-block;
}
.hero { display: flex; gap: 24px; align-items: center; padding: 36px 0; }
.hero h1 { font-size: 28px; margin-bottom: 8px; }
.hero p { color: var(--muted); margin-bottom: 16px; }
.grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 18px; }
.card {
  background: var(--card); padding: 18px; border-radius: var(--radius);
  box-shadow: 0 6px 18px rgba(15,23,42,0.06);
}
.course-title { font-size: 18px; margin-bottom: 8px; }
.course-desc { color: var(--muted); font-size: 14px; margin-bottom: 12px; }
.footer { padding: 24px 0; color: var(--muted); font-size: 14px; text-align:center;}
.input, textarea, select {
  padding: 10px; border-radius: 8px; border: 1px solid #e6e9ef; width: 100%;
}
.small { font-size: 14px; color: var(--muted); }
@media (max-width: 720px) {
  .hero { flex-direction: column; align-items: flex-start; }
  .nav a:not(.btn) { display: none; }
}







comon- const COURSES = [
  { id: "gardening-basic", name: "Gardening Basics", desc: "Plant care, pruning, and soil prep.", price: 350 },
  { id: "domestic-care", name: "Domestic Care & Cleaning", desc: "Practical household cleaning and safety.", price: 420 },
  { id: "food-prep", name: "Basic Food Prep", desc: "Safe, affordable meals and portioning.", price: 390 },
];

function formatZAR(n) {
  return "R" + Number(n).toLocaleString("en-ZA");
}

function renderCourses(targetId, limit) {
  const target = document.getElementById(targetId);
  if (!target) return;
  const list = limit ? COURSES.slice(0, limit) : COURSES;
  target.innerHTML = list
    .map(
      (c) => `
    <div class="card">
      <h3 class="course-title">${c.name}</h3>
      <div class="course-desc">${c.desc}</div>
      <div class="small">Price per person: ${formatZAR(c.price)}</div>
      <div style="margin-top:10px"><a class="btn" href="courses-detail.html?id=${c.id}">View</a></div>
    </div>
  `
    )
    .join("");
}

document.addEventListener("DOMContentLoaded", () => {
  renderCourses("coursesGrid", 3);
  renderCourses("coursesGridAll");

  const select = document.getElementById("courseSelect");
  if (select) {
    COURSES.forEach((c) =>
      select.insertAdjacentHTML("beforeend", `<option value="${c.id}">${c.name} — ${formatZAR(c.price)}</option>`)
    );
  }

  const calcBtn = document.getElementById("calcBtn");
  if (calcBtn) {
    calcBtn.addEventListener("click", () => {
      const pid = document.getElementById("courseSelect").value || COURSES[0].id;
      const n = Number(document.getElementById("participants").value) || 1;
      const course = COURSES.find((c) => c.id === pid);
      const total = n * course.price;
      document.getElementById("calcResult").textContent = `${formatZAR(total)} (${n} x ${formatZAR(course.price)})`;
    });
  }

  const params = new URLSearchParams(location.search);
  const id = params.get("id");
  if (id) {
    const course = COURSES.find((c) => c.id === id);
    if (course) {
      document.getElementById("courseName").textContent = course.name;
      document.getElementById("courseDesc").textContent = course.desc;
      document.getElementById("coursePrice").textContent = formatZAR(course.price);

      const calcDetail = document.getElementById("calcDetail");
      if (calcDetail) {
        calcDetail.addEventListener("click", () => {
          const n = Number(document.getElementById("numStudents").value) || 1;
          document.getElementById("detailResult").textContent = `${formatZAR(n * course.price)} (${n} x ${formatZAR(
            course.price
          )})`;
        });
      }
    }
  }

  const sendBtn = document.getElementById("sendBtn");
  if (sendBtn) {
    sendBtn.addEventListener("click", () => {
      const name = document.getElementById("name").value.trim();
      const email = document.getElementById("email").value.trim();
      const msg = document.getElementById("message").value.trim();
      const el = document.getElementById("sendResult");
      if (!name || !email || !msg) {
        el.textContent = "Please complete all fields.";
        return;
      }
      el.textContent = "Thanks — your message has been received.";
    });
  }
});















calc- <!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Course Fee Calculator — Empowering the Nation</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="header">
    <div class="container nav">
      <div class="brand">
        <img src="logo.jpg" alt="logo" />
        <div><strong>Empowering the Nation</strong><div class="small">Course Fee Calculator</div></div>
      </div>
      <nav>
        <a href="index.html">Home</a>
        <a href="courses.html">Courses</a>
        <a href="calculation.html" class="btn">Calculator</a>
        <a href="contact.html">Contact</a>
      </nav>
    </div>
  </header>

  <main class="container">
    <h1>Course Fee Calculator</h1>
    <p class="small">Select a course, number of students, and we’ll calculate your total including VAT (15%).</p>

    <div class="card" style="max-width:500px">
      <label class="small">Select Course</label>
      <select id="calcCourse" class="input"></select>

      <label class="small">Number of Students</label>
      <input id="calcStudents" class="input" type="number" min="1" value="1" />

      <div style="height:12px"></div>
      <button id="calcTotalBtn" class="btn">Calculate Total</button>

      <div id="calcOutput" style="margin-top:16px;font-weight:600"></div>
    </div>
  </main>

  <footer class="container footer">© 2025 Empowering the Nation</footer>
  <script src="common.js"></script>
</body>
</html>
















  // --- Calculation Page Logic (with VAT) ---
  const VAT_RATE = 0.15;

  const calcCourse = document.getElementById("calcCourse");
  const calcStudents = document.getElementById("calcStudents");
  const calcTotalBtn = document.getElementById("calcTotalBtn");
  const calcOutput = document.getElementById("calcOutput");

  if (calcCourse && calcTotalBtn) {
    // Populate dropdown
    COURSES.forEach((c) => {
      calcCourse.insertAdjacentHTML("beforeend", `<option value="${c.id}">${c.name} — ${formatZAR(c.price)}</option>`);
    });

    calcTotalBtn.addEventListener("click", () => {
      const selectedId = calcCourse.value;
      const course = COURSES.find((c) => c.id === selectedId);
      const students = Number(calcStudents.value) || 1;

      const subtotal = students * course.price;
      const vat = subtotal * VAT_RATE;
      const total = subtotal + vat;

      calcOutput.innerHTML = `
        <div>Subtotal (${students} x ${formatZAR(course.price)}): <strong>${formatZAR(subtotal)}</strong></div>
        <div>VAT (15%): <strong>${formatZAR(vat)}</strong></div>
        <hr style="margin:10px 0;">
        <div>Total (incl. VAT): <strong style="color:var(--accent)">${formatZAR(total)}</strong></div>
      `;
    });
  }















  idnx,courses,contact        <a href="calculation.html">Calculator</a>


