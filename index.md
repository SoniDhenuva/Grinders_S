---
layout: post 
title: Open Coding Society
description: An Open Pathway to Computer Science
image: /images/mario_animation.png
hide: true
---

## About

Empower yourself to solve real-world problems, unlock creativity, and open doors to every field—because coding is the language of innovation.

> Invest in your technical skills through Project-based learning.

<div style="display: flex; align-items: flex-start; justify-content: center; gap: 40px; flex-wrap: wrap;">

  <!-- Logo -->
  <div style="text-align: center;">
    <img src="{{site.baseurl}}/images/logo-framed.png" alt="Logo" style="width: 180px; max-width: 100%;">
  </div>

  <!-- QR Code -->
  <div style="text-align: center;">
    <img src="{{site.baseurl}}/images/course-brag/qr.png" alt="QR Code" style="width: 180px; max-width: 100%;">
  </div>

  <!-- Socials -->
  <div style="min-width: 220px;">
    <ul style="list-style: none; padding: 0; font-size: 1.1em;">
      <li>
        <img class="social-icon" src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/gmail.svg" alt="Gmail" style="width: 20px; vertical-align: middle; margin-right: 8px;">
        <a href="mailto:open.coding.society@gmail.com">open.coding.society@gmail.com</a>
      </li>
      <li>
        <img class="social-icon" src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/linkedin.svg" alt="LinkedIn" style="width: 20px; vertical-align: middle; margin-right: 8px;">
        <a href="https://linkedin.com/company/open-coding-society" target="_blank">LinkedIn</a>
      </li>
      <li>
        <img class="social-icon" src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/x.svg" alt="X" style="width: 20px; vertical-align: middle; margin-right: 8px;">
        <a href="https://x.com/Open_Coding" target="_blank">@Open_Coding</a>
      </li>
      <li>
        <img class="social-icon" src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/youtube.svg" alt="YouTube" style="width: 20px; vertical-align: middle; margin-right: 8px;">
        <a href="https://www.youtube.com/@OpenCodingSociety" target="_blank">@OpenCodingSociety</a>
      </li>
    </ul>
  </div>
</div>
<br>
<br>
<br>
<table border="1" cellspacing="0" cellpadding="8">
    <tr>
      <th>Team</th>
      <th>Role</th>
      <th>GitHub</th>
    </tr>
    <tr>
      <td>Nora</td>
      <td></td>
      <td><a href="https://github.com/NoraTheTurtle" target="_blank">NoraTheTurtle</a></td>
    </tr>
    <tr>
      <td>Avika</td>
      <td></td>
      <td><a href="https://github.com/avikaprasad22" target="_blank">Avikaprasad22</a></td>
    </tr>
    <tr>
      <td>Soni</td>
      <td></td>
      <td><a href="https://github.com/SoniDhenuva" target="_blank">SoniDhenuva</a></td>
    </tr>
    <tr>
      <td>Nolan</td>
      <td></td>
      <td><a href="https://github.com/nulxn" target="_blank">Nulxn</a></td>
    </tr>
    <tr>
      <td>Yuva</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Yash</td>
      <td></td>
      <td></td>
    </tr>
</table>


<br>


<!-- Feedback Button + Modal -->
<style>
  #feedback-btn {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background-color: #2563eb;
    color: white;
    border: none;
    border-radius: 9999px;
    padding: 12px 20px;
    font-size: 14px;
    font-weight: 500;
    cursor: pointer;
    box-shadow: 0 2px 6px rgba(0, 0, 0, 0.2);
    transition: background-color 0.2s ease-in-out;
    z-index: 1000;
  }

  #feedback-btn:hover {
    background-color: #1e40af;
  }

  #feedback-modal {
    display: none;
    position: fixed;
    bottom: 80px;
    right: 20px;
    background: #1f2937;
    color: white;
    border-radius: 16px;
    padding: 20px;
    width: 320px;
    max-width: 90vw;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.4);
    border: 1px solid #4b5563;
    z-index: 1000;
    animation: slideIn 0.2s ease-out;
    box-sizing: border-box;
  }

  #feedback-modal h4 {
    color: white;
    font-size: 16px;
    font-weight: 600;
    margin-bottom: 12px;
    text-align: center;
    border-bottom: 1px solid #4b5563;
    padding-bottom: 8px;
  }

  #feedback-modal textarea,
  #feedback-modal input {
    width: 100%;
    margin-bottom: 12px;
    padding: 10px;
    font-size: 14px;
    color: white;
    background: #374151;
    border-radius: 8px;
    border: 1px solid #6b7280;
    box-sizing: border-box;
  }

  #feedback-modal textarea::placeholder,
  #feedback-modal input::placeholder {
    color: #9ca3af;
  }

  #feedback-modal textarea:focus,
  #feedback-modal input:focus {
    outline: none;
    border-color: #3b82f6;
  }

  #feedback-modal button {
    background-color: #3b82f6;
    color: white;
    border: none;
    border-radius: 8px;
    padding: 10px;
    width: 100%;
    font-weight: 500;
    transition: background-color 0.2s ease-in-out;
  }

  #feedback-modal button:hover {
    background-color: #2563eb;
  }

  #feedback-modal-close {
    position: absolute;
    top: 10px;
    right: 12px;
    font-size: 16px;
    font-weight: bold;
    color: #9ca3af;
    cursor: pointer;
  }

  #feedback-modal-close:hover {
    color: white;
  }

  #feedback-success,
  #feedback-error {
    font-size: 13px;
    text-align: center;
    margin-top: 12px;
  }

  #feedback-success {
    color: #10b981;
  }

  #feedback-error {
    color: #ef4444;
  }

  @keyframes slideIn {
    from {
      transform: translateY(20px);
      opacity: 0;
    }
    to {
      transform: translateY(0);
      opacity: 1;
    }
  }

  #feedback-modal select {
    width: 100%;
    margin-bottom: 12px;
    padding: 10px;
    font-size: 14px;
    color: white;
    background: #374151;
    border-radius: 8px;
    border: 1px solid #6b7280;
    box-sizing: border-box;
    appearance: none;
  }

  #feedback-modal select:focus {
    outline: none;
    border-color: #3b82f6;
  }

  #feedback-modal select option {
    background-color: #1f2937;
    color: white;
  }
</style>

<!-- Feedback Button & Modal -->
<button id="feedback-btn">Tell us how we can improve!</button>

<div id="feedback-modal">
  <div id="feedback-modal-close">✕</div>
  <h4>Submit Feedback</h4>
  <select id="feedback-type" required>
    <option value="">Select Inquiry Type</option>
    <option value="Bug">Bug</option>
    <option value="Feature Request">Feature Request</option>
    <option value="Inquiry">Inquiry</option>
    <option value="Other">Other</option>
  </select>
  <input type="text" id="feedback-title" placeholder="Title" required />
  <textarea id="feedback-body" rows="4" placeholder="Your suggestion..." required></textarea>
  <button id="feedback-submit">Submit</button>
  <div id="feedback-success" style="display:none;">✅ Thanks for your feedback!</div>
  <div id="feedback-error" style="display:none;">⚠️ Something went wrong.</div>
</div>

<script type="module">
  import { javaURI } from '{{ site.baseurl }}/assets/js/api/config.js';
  import { pythonURI } from '{{ site.baseurl }}/assets/js/api/config.js';

  const btn = document.getElementById("feedback-btn");
  const modal = document.getElementById("feedback-modal");
  const closeBtn = document.getElementById("feedback-modal-close");
  const submitBtn = document.getElementById("feedback-submit");
  const successMsg = document.getElementById("feedback-success");
  const errorMsg = document.getElementById("feedback-error");
  console.log(window.user);

  btn.onclick = () => {
    modal.style.display = "block";
    successMsg.style.display = "none";
    errorMsg.style.display = "none";
  };

  closeBtn.onclick = () => {
    modal.style.display = "none";
  };

  submitBtn.onclick = async () => {
    const title = document.getElementById("feedback-title").value.trim();
    const body = document.getElementById("feedback-body").value.trim();
    const type = document.getElementById("feedback-type").value;

    if (!title || !body) {
      alert("Please fill in both fields.");
      return;
    }

    const githubUsername = window.user?.uid || "Anonymous"; // fallback if not logged in
    
    console.log("Payload:", { title, body, type, uid: githubUsername });
    
    try {
      const res = await fetch(`${pythonURI}/api/feedback/`, {
        method: "POST",
        headers: {
          "Content-Type": "application/json"
        },
        body: JSON.stringify({ title, body, type, uid: githubUsername })
      });

      if (res.ok) {
        successMsg.style.display = "block";
        errorMsg.style.display = "none";
        document.getElementById("feedback-title").value = "";
        document.getElementById("feedback-body").value = "";
      } else {
        throw new Error();
      }
    } catch (err) {
      successMsg.style.display = "none";
      errorMsg.style.display = "block";
    }
  };
</script>
