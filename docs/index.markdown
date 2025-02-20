---
layout: default
title: Hochzeit Nadia & Erica
---

<section>
  <h2>Unsere Geschichte</h2>
  <p>Wir lernten uns vor 9 Jahren kennen, als wir einfach nur Spaß haben wollten. Was als unbeschwerter Moment begann, entwickelte sich zu einer tiefen und unerschütterlichen Liebe. Seitdem teilen wir Höhen und Tiefen, lachen, wachsen und leben ein gemeinsames Leben voller Abenteuer und Glück. Jetzt wollen wir den nächsten Schritt gehen und unsere Liebe mit allen feiern.</p>
  <img src="hochzeit.jpeg" alt="Foto von Nadia & Erica">
</section>

<section>
  <h2>Der große Tag</h2>
  <h3>**13.09.2025**</h3>
  <div id="countdown"></div>
  <hr>
</section>

<section>
  <h3>Details der Feier:</h3>
  <ul>
    <li><strong>Datum:</strong> 13. September 2025</li>
    <li><strong>Uhrzeit:</strong> Wird noch bekannt gegeben</li>
    <li><strong>Ort:</strong> Der genaue Ort wird noch bekannt gegeben. Ein Link mit dem Standort folgt.</li>
  </ul>
</section>

<section>
  <h3>Programm des Tages</h3>
  <p>Der Ablauf und die Zeiten werden euch bald mitgeteilt! 🥂</p>
</section>

<section>
  <h3>Danke, dass ihr dabei seid!</h3>
  <p>Wir freuen uns unglaublich, diesen besonderen Tag mit euch zu teilen und gemeinsam mit euch zu feiern. Eure Anwesenheit bedeutet viel! Bitte teilt uns mit, ob ihr kommen könnt.</p>
</section>

<script>
  const targetDate = new Date("2025-09-13T00:00:00").getTime();
  const interval = setInterval(() => {
    const now = new Date().getTime();
    const distance = targetDate - now;

    if (distance < 0) {
      clearInterval(interval);
      document.getElementById("countdown").innerHTML = "Der große Tag ist da! 🎉";
      return;
    }

    const days = Math.floor(distance / (1000 * 60 * 60 * 24));
    const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
    const seconds = Math.floor((distance % (1000 * 60)) / 1000);

    document.getElementById("countdown").innerHTML =
      days + " Tage " + hours + " Stunden " + minutes + " Minuten " + seconds + " Sekunden ";
  }, 1000);
</script>
