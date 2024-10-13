<div class="support-resistance" id="levels">
        <div class="level" id="support1">دعم 1: </div>
        <div class="level" id="support2">دعم 2: </div>
        <div class="level" id="support3">دعم 3: </div>
        <div class="level" id="pivotLevel">Pivot: </div>
        <div class="level" id="resistance1">مقاومة 1: </div>
        <div class="level" id="resistance2">مقاومة 2: </div>
        <div class="level" id="resistance3">مقاومة 3: </div>
    </div>
</div>

<script>
    function calculate() {
        const high = parseFloat(document.getElementById('high').value);
        const low = parseFloat(document.getElementById('low').value);
        const close = parseFloat(document.getElementById('close').value);

        if (!isNaN(high) && !isNaN(low) && !isNaN(close)) {
            const pivot = (high + low + (2 * close)) / 4;
            const support1 = (2 * pivot) - high;
            const support2 = pivot - (high - low);
            const support3 = low + 2 * (pivot - high);
            const resistance1 = (2 * pivot) - low;
            const resistance2 = pivot + (high - low);
            const resistance3 = high + 2 * (pivot - low);
            
            document.getElementById('result').innerText = قيمة Pivot هي: ${pivot.toFixed(2)};
            document.getElementById('result').style.display = 'block';
            
            document.getElementById('support1').innerText = دعم 1: ${support1.toFixed(2)};
            document.getElementById('support2').innerText = دعم 2: ${support2.toFixed(2)};
            document.getElementById('support3').innerText = دعم 3: ${support3.toFixed(2)};
            document.getElementById('resistance1').innerText = مقاومة 1: ${resistance1.toFixed(2)};
            document.getElementById('resistance2').innerText = مقاومة 2: ${resistance2.toFixed(2)};
            document.getElementById('resistance3').innerText = مقاومة 3: ${resistance3.toFixed(2)};
            
            document.getElementById('levels').style.display = 'flex'; // عرض مستويات الدعم والمقاومة
        } else {
            document.getElementById('result').innerText = 'يرجى إدخال جميع القيم بشكل صحيح.';
            document.getElementById('result').style.display = 'block';
            document.getElementById('levels').style.display = 'none'; // إخفاء مستويات الدعم والمقاومة
        }
    }
</script>

</body>
</html>
