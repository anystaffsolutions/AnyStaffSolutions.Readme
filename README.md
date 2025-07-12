<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AnyStaff Solutions</title>
  <style>
    * { box-sizing: border-box; }
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-color: #f2f2f2;
      color: #333;
    }
    header {
      background-color: #004aad;
      color: #fff;
      padding: 2em;
      text-align: center;
    }
    nav {
      background: #003e7e;
      padding: 1em;
      text-align: center;
    }
    nav a {
      color: #fff;
      margin: 0 1em;
      text-decoration: none;
      font-weight: bold;
    }
    .hero {
      background: #e6f0ff;
      padding: 2em;
      text-align: center;
    }
    .hero h2 { margin-bottom: 0.5em; }
    .hero a {
      display: inline-block;
      margin-top: 1em;
      padding: 0.75em 1.5em;
      background: #004aad;
      color: #fff;
      text-decoration: none;
      border-radius: 8px;
    }
    .container {
      max-width: 1000px;
      margin: 2em auto;
      padding: 0 1em;
    }
    .job-listing {
      background: white;
      padding: 1em;
      margin-bottom: 1em;
      border-radius: 8px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }
    .apply-btn {
      display: inline-block;
      padding: 0.5em 1em;
      background: #004aad;
      color: white;
      text-decoration: none;
      border-radius: 5px;
      margin-top: 0.5em;
    }
    .testimonial, .client, .apply-form, .try-career {
      background: white;
      padding: 1em;
      border-radius: 8px;
      margin-top: 2em;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }
    label { display: block; margin-top: 1em; }
    input, textarea {
      width: 100%;
      padding: 0.5em;
      border: 1px solid #ccc;
      border-radius: 6px;
    }
    #chat-box {
      height: 300px;
      overflow-y: auto;
      border: 1px solid #ccc;
      padding: 1em;
      border-radius: 8px;
      background: #fafafa;
      margin-top: 2em;
    }
    .message { margin-bottom: 1em; }
    .user { color: #000; font-weight: bold; }
    .ai { color: #004aad; }
    #input-area {
      display: flex;
      gap: 0.5em;
      margin-top: 1em;
    }
    #user-input {
      flex-grow: 1;
      padding: 0.75em;
      border: 1px solid #ccc;
      border-radius: 6px;
    }
    #send-btn {
      padding: 0.75em 1em;
      background: #004aad;
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
    }
    iframe {
      width: 100%;
      height: 315px;
      border: none;
      margin-top: 1em;
      border-radius: 6px;
    }
    footer {
      text-align: center;
      background: #333;
      color: #fff;
      padding: 1em;
      margin-top: 3em;
    }
  </style>
</head>
<body>
  <header>
    <h1>AnyStaff Solutions</h1>
    <p>Staffing Indiana’s Warehouses with Heart, AI, and Human Power</p>
  </header>  <nav>
    <a href="#jobs">Jobs</a>
    <a href="#ai">AI Assistant</a>
    <a href="#try-career">Try a Career</a>
    <a href="#apply">Apply</a>
    <a href="#client">Hire</a>
    <a href="#contact">Contact</a>
  </nav>  <section class="hero">
    <h2>Connecting Indiana’s Workforce to Opportunity — One Shift at a Time</h2>
    <a href="#apply">Apply Now</a>
  </section>  <div class="container">
    <section id="jobs">
      <h2>Job Openings</h2>
      <div class="job-listing">
        <h3>Forklift Operator - Plainfield, IN</h3>
        <p>PIT certified, high-pace loading dock, 2nd shift</p>
        <p><strong>$18/hr</strong></p>
        <a class="apply-btn" href="#apply">Apply</a>
      </div>
      <div class="job-listing">
        <h3>Warehouse Labor - Indianapolis</h3>
        <p>Pick/pack/sort, climate controlled</p>
        <p><strong>$16.50/hr</strong></p>
        <a class="apply-btn" href="#apply">Apply</a>
      </div>
    </section><section id="ai">
  <h2>AI Support Chat</h2>
  <div id="chat-box">
    <div class="message ai"><strong class="ai">AI:</strong> Hi! I’m your support assistant. Talk to me about burnout, safety, ideas, or shift swaps.</div>
  </div>
  <div id="input-area">
    <input type="text" id="user-input" placeholder="Type here...">
    <button id="send-btn">Send</button>
  </div>
</section>

<section id="try-career" class="try-career">
  <h2>Try a Career: Safety Preview + OSHA Training</h2>
  <p>Explore what your next role might feel like before you even start. Watch safety intro videos, understand your PPE requirements, and preview warehouse working conditions.</p>
  <ul>
    <li>👷 Required Gear: Hard Hat, Hi-Vis Vest, Gloves, Steel-Toe Boots</li>
    <li>📋 OSHA Safety Training Essentials</li>
    <li>📹 Interactive Preview Experience Below</li>
  </ul>
  <iframe src="https://www.youtube.com/embed/qfALUjwhD8k" title="Forklift Safety Training Video" allowfullscreen></iframe>
  <p><em>Video: OSHA Forklift Safety Guide (Placeholder — replace with your custom content)</em></p>
</section>

<section id="apply" class="apply-form">
  <h2>Quick Apply</h2>
  <form>
    <label for="name">Full Name</label>
    <input type="text" id="name">
    <label for="email">Email</label>
    <input type="email" id="email">
    <label for="job">Job Interest</label>
    <input type="text" id="job">
    <label for="resume">Paste Resume (optional)</label>
    <textarea id="resume"></textarea>
  </form>
</section>

<section id="client" class="client">
  <h2>Need Staff?</h2>
  <p>If you're a warehouse or logistics manager in Indiana looking for PIT-certified, safety-trained, high-performing talent — we got you covered.</p>
  <p>Email Megan Phillips at <a href="mailto:anystaffsolutions@gmail.com">anystaffsolutions@gmail.com</a></p>
</section>

<section class="testimonial">
  <h2>What Our Workers Say</h2>
  <p>“The AI chat helped me swap shifts when I was overwhelmed. It felt like someone was actually listening.” – Chris D., Greenwood</p>
</section>

<section id="contact">
  <h2>Contact Us</h2>
  <p><strong>Founder:</strong> Megan Phillips</p>
  <p>Email: <a href="mailto:anystaffsolutions@gmail.com">anystaffsolutions@gmail.com</a></p>
  <p>Phone: <a href="tel:3174897113">317-489-7113</a></p>
</section>

  </div>  <footer>
    <p>&copy; 2025 AnyStaff Solutions. Built with Heart, Backed by AI.</p>
  </footer>  <script>
    const chatBox = document.getElementById('chat-box');
    const userInput = document.getElementById('user-input');
    const sendBtn = document.getElementById('send-btn');

    function appendMessage(sender, text) {
      const message = document.createElement('div');
      message.classList.add('message');
      message.innerHTML = `<strong class="${sender.toLowerCase()}">${sender}:</strong> ${text}`;
      chatBox.appendChild(message);
      chatBox.scrollTop = chatBox.scrollHeight;
    }

    function getAIResponse(input) {
      const msg = input.toLowerCase();
      if (msg.includes('burnout')) {
        return "Thanks for checking in. Your well-being is our priority. I'll flag this for scheduling and swap support.";
      } else if (msg.includes('swap') || msg.includes('day off')) {
        return "Noted. Let’s find a teammate with matching availability. I’ll follow up shortly.";
      } else if (msg.includes('idea') || msg.includes('feedback')) {
        return "Got it. Your ideas help us grow. We may contact you if your suggestion fits the client’s needs. Thank you for innovating.";
      } else if (msg.includes('safety')) {
        return "Safety Tip: Stay alert. Use PPE. Follow forklift zones. Report any hazard immediately.";
      } else {
        return "You are heard, understood, and supported. AnyStaff stands by your growth and your voice. Keep sharing."
      }
    }

    sendBtn.addEventListener('click', () => {
      const input = userInput.value.trim();
      if (!input) return;
      appendMessage('User', input);
      userInput.value = '';
      setTimeout(() => {
        const response = getAIResponse(input);
        appendMessage('AI', response);
      }, 500);
    });
  </script></body>
</html>

