
function redirectToNextPage() {
    window.location.href = "next.html";
  }
  
  
  function calculateAverage() {
    const subjects = ["mathsMarks", "pythonMarks", "dsaMarks", "mpMarks", "mdmMarks", "oecMarks"];
    let marks = subjects.map(id => parseFloat(document.getElementById(id).value) || 0);
  
    marks.sort((a, b) => b - a);
    const bestFive = marks.slice(0, 5);
    const sum = bestFive.reduce((acc, mark) => acc + mark, 0);
    const average = sum / 5;
  
    const resultDiv = document.getElementById("result");
    resultDiv.innerHTML = `<p class="result-text">${average > 80 ? "Excellent!" : "Good!"} Your average is ${average.toFixed(2)}%</p>`;
    resultDiv.classList.add("show");
  
    resultDiv.scrollIntoView({ behavior: "smooth" });
  }
  
  document.querySelectorAll("input").forEach(input => {
    input.addEventListener("focus", function () {
        this.style.borderColor = "#4CAF50";
        this.style.boxShadow = "0 0 5px #4CAF50";
    });
  
    input.addEventListener("blur", function () {
        this.style.borderColor = "#ddd";
        this.style.boxShadow = "none";
    });
  });
  