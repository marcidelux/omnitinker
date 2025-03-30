---
title: CV 📄
icon: fas fa-file-pdf
order: 3
---

<div id="pdf-viewer"></div>

<script src="/assets/lib/pdfjs/build/pdf.js"></script>
<script>
  document.addEventListener("DOMContentLoaded", function () {
    const url = '/assets/files/cv.pdf';

    const loadingTask = pdfjsLib.getDocument(url);
    loadingTask.promise.then(pdf => {
      const container = document.getElementById('pdf-viewer');

      for (let pageNum = 1; pageNum <= pdf.numPages; pageNum++) {
        pdf.getPage(pageNum).then(page => {
          const canvas = document.createElement("canvas");
          container.appendChild(canvas);
          const context = canvas.getContext("2d");

          const viewport = page.getViewport({ scale: 1.5 });
          canvas.height = viewport.height;
          canvas.width = viewport.width;

          page.render({ canvasContext: context, viewport });
        });
      }
    });
  });
</script>