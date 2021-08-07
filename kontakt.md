---
layout: textcontent
---

Für Fragen, Anregungen, Austausch usw. haben wir eine Mailingliste und eine LINE-Gruppe.

### Mailingliste

Sende eine E-Mail an <span id="inb4mail" title="Nicht kopierbar."></span>lists.kit.edu, um zur Mailingliste hinzugefügt zu werden.

### LINE-Gruppe

![QR-Code](/assets/img/line_qr.jpg)
<br><span id="ll"></span>

<!-- undo CSS shenanigans w/ JS shenanigans-->
<script>
ibm = document.getElementById('inb4mail');
ibm.innerHTML = getComputedStyle(
    ibm, ':before'
).getPropertyValue(
    'content'
).replace(
    'р', 'p'
).replaceAll(
    '"', ''
);
ibm.title = '';
ibm.id = '';

ll_spn = document.getElementById('ll');
ll_base = 'https://line.me/R/ti/g/';
ll_id = 'G_GInVdWj8';
ll_a = document.createElement('a');
ll_a.href = ll_base + ll_id;
ll_spn.appendChild(ll_a);
ll_a.innerHTML = 'Link zur LINE-Gruppe';
</script>
<!-- end of shenanigans -->
