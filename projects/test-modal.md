
---
layout: default
title: Test Modal
permalink: /projects/test-modal/
---

# Test Modal Page

Click the button below to test a modal popup on GitHub Pages.

<button class="project-modal-btn" onclick="openModal('demoModal')">
  Open Test Modal
</button>

<!-- Modal -->
<div id="demoModal" class="project-modal">
  <div class="project-modal-content">
    <span class="modal-close" onclick="closeModal('demoModal')">&times;</span>
    <h2>Modal Working!</h2>
    <p>
      If you can see this, then modals work perfectly on GitHub Pages.
      You can put **images**, **videos**, **text**, or anything else here.
    </p>
  </div>
</div>

<style>
.project-modal {
  display: none;
  position: fixed;
  z-index: 9999;
  padding-top: 80px;
  left: 0; top: 0;
  width: 100%; height: 100%;
  background: rgba(0,0,0,0.7);
}

.project-modal-content {
  background: #fff;
  margin: auto;
  padding: 20px;
  width: 70%;
  max-width: 700px;
  border-radius: 10px;
  box-shadow: 0 0 20px rgba(0,0,0,0.3);
}

.project-modal-btn {
  padding: 10px 18px;
  background: #0077ff;
  color: white;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}

.project-modal-btn:hover {
  background: #005fcc;
}

.modal-close {
  float: right;
  font-size: 28px;
  cursor: pointer;
  font-weight: bold;
}
</style>

<script>
function openModal(id) {
  document.getElementById(id).style.display = 'block';
}

function closeModal(id) {
  document.getElementById(id).style.display = 'none';
}

window.onclick = function(e) {
  document.querySelectorAll('.project-modal').forEach(m => {
    if (e.target === m) m.style.display = "none";
  });
};
</script>
