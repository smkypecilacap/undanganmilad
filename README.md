<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Undangan Milad SMK YPE Cilacap</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Montserrat', sans-serif;
            background-color: #0f172a;
            background-image: url("data:image/svg+xml,<svg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'><g fill='none' fill-rule='evenodd'><g fill='#1e293b' fill-opacity='0.4'><path d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/></g></g></svg>");
        }
        .title-font {
            font-family: 'Playfair Display', serif;
        }
        .gold-gradient {
            background: linear-gradient(to right, #fbbf24, #d97706);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .glass-panel {
            background: rgba(30, 41, 59, 0.7);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        .glow {
            box-shadow: 0 0 15px rgba(251, 191, 36, 0.3);
        }
        .fade-in {
            animation: fadeIn 1.5s ease-in-out;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body class="min-h-screen flex items-center justify-center p-4">

    <!-- Container Utama -->
    <div class="glass-panel w-full max-w-md rounded-2xl shadow-2xl overflow-hidden relative fade-in">
        
        <!-- Header Image / Ornament -->
        <div class="h-40 bg-gradient-to-r from-slate-900 via-slate-800 to-slate-900 flex flex-col items-center justify-center relative">
            <div class="absolute inset-0 opacity-20" style="background-image: radial-gradient(circle at center, #fbbf24 1px, transparent 1px); background-size: 20px 20px;"></div>
            <div class="text-center z-10 px-4">
                <i class="fas fa-crown text-amber-400 text-3xl mb-2 animate-bounce"></i>
                <h3 class="text-amber-100 text-xs tracking-[0.3em] font-semibold mb-3 uppercase">Undangan Khusus Untuk:</h3>
                <div id="guest-name" class="text-white text-xl font-bold border-y border-amber-500/30 py-1 px-4 inline-block bg-slate-900/50 rounded-sm">
                    Tamu Undangan
                </div>
            </div>
        </div>

        <!-- Isi Undangan -->
        <div class="p-8 text-center">
            <p class="text-slate-400 text-sm mb-2 italic">Assalamu’alaikum Warahmatullahi Wabarakatuh</p>
            <p class="text-slate-300 text-sm mb-6">Tanpa mengurangi rasa hormat, kami mengundang <span class="guest-name-inline font-bold text-amber-400">Saudara/i</span> untuk hadir dalam acara:</p>

            <h1 class="title-font text-4xl font-bold text-white mb-2 leading-tight">MILAD KE-52<br><span class="gold-gradient">SMK YPE CILACAP</span></h1>
            
            <!-- Subjudul -->
            <p class="text-amber-200 text-xs font-semibold tracking-wider mb-6 px-2 uppercase">"52 Tahun SMK YPE Cilacap mengabdi untuk negeri"</p>
            
            <div class="h-px w-24 bg-amber-500 mx-auto mb-6 opacity-50"></div>

            <!-- Detail Acara -->
            <div class="space-y-4 text-left bg-slate-800/50 p-5 rounded-xl border border-slate-700">
                <div class="flex items-start gap-4">
                    <div class="w-10 h-10 rounded-full bg-slate-700 flex items-center justify-center flex-shrink-0 text-amber-400">
                        <i class="far fa-calendar-alt"></i>
                    </div>
                    <div>
                        <p class="text-xs text-slate-400 uppercase tracking-wider">Hari & Tanggal</p>
                        <p class="text-white font-semibold">Selasa, 3 Februari 2026</p>
                    </div>
                </div>

                <div class="flex items-start gap-4">
                    <div class="w-10 h-10 rounded-full bg-slate-700 flex items-center justify-center flex-shrink-0 text-amber-400">
                        <i class="far fa-clock"></i>
                    </div>
                    <div>
                        <p class="text-xs text-slate-400 uppercase tracking-wider">Waktu</p>
                        <p class="text-white font-semibold">07.30 - Selesai</p>
                        <p class="text-xs text-amber-500">(Close Gate 08.30)</p>
                    </div>
                </div>

                <div class="flex items-start gap-4">
                    <div class="w-10 h-10 rounded-full bg-slate-700 flex items-center justify-center flex-shrink-0 text-amber-400">
                        <i class="fas fa-map-marker-alt"></i>
                    </div>
                    <div>
                        <p class="text-xs text-slate-400 uppercase tracking-wider">Lokasi</p>
                        <p class="text-white font-semibold">Halaman SMK YPE Cilacap</p>
                        <p class="text-xs text-slate-400">Jl. Dr. Sutomo No. 8 Cilacap</p>
                    </div>
                </div>
            </div>

            <!-- Countdown Timer -->
            <div class="mt-6 mb-2">
                <p class="text-xs text-slate-400 mb-2">Menuju Acara:</p>
                <div class="grid grid-cols-4 gap-2" id="countdown"></div>
            </div>

            <!-- Gabungan Kata Mutiara -->
            <p class="text-slate-300 text-sm mt-6 mb-8 italic">
                "Mari pererat tali silaturahmi dan kenang masa-masa berjuang bersama. <br>
                <span class="text-amber-400 font-semibold italic">Alumni seduluran selawase</span>"
            </p>

            <!-- Action Buttons -->
            <div class="grid grid-cols-1 gap-3">
                <button onclick="openMap()" class="w-full py-3 bg-slate-700 hover:bg-slate-600 text-white rounded-lg font-semibold transition flex items-center justify-center gap-2 border border-slate-600">
                    <i class="fas fa-map-marked-alt"></i> Lokasi Google Maps
                </button>
                <button onclick="confirmWA()" class="w-full py-3 bg-green-600 hover:bg-green-500 text-white rounded-lg font-semibold transition glow flex items-center justify-center gap-2 shadow-lg shadow-green-900/50">
                    <i class="fab fa-whatsapp"></i> Konfirmasi Kehadiran
                </button>
            </div>
            
            <div class="mt-6 pt-4 border-t border-slate-700">
                <button onclick="copyInvitation()" class="text-amber-500 text-sm hover:text-amber-400 underline decoration-dotted underline-offset-4">
                    <i class="far fa-copy"></i> Salin Teks Pesan WhatsApp
                </button>
                <p id="copyFeedback" class="text-green-400 text-xs mt-1 hidden">Teks disalin sesuai nama tamu!</p>
            </div>
        </div>

        <div class="bg-slate-900 p-3 text-center border-t border-slate-800">
            <p class="text-xs text-slate-500">Panitia Milad SMK YPE Cilacap ke-52</p>
        </div>
    </div>

    <!-- Hidden Text Area for Copying -->
    <textarea id="invitationText" class="hidden">
*UNDANGAN MILAD SMK YPE CILACAP KE-52*
"52 Tahun SMK YPE Cilacap mengabdi untuk negeri"

Assalamu’alaikum Wr. Wb.

Yth. [NAMA],
Kami mengundang Anda untuk hadir meramaikan acara MILAD Sekolah kita yang ke-52. 

🗓 Hari/Tgl: Selasa, 3 Februari 2026
⏰ Pukul: 07.30 - Selesai (close gate 08.30)
📍 Tempat: Halaman SMK YPE Cilacap, Jl. Dr. Sutomo No. 8 Cilacap

Mari pererat tali silaturahmi dan kenang masa-masa berjuang bersama. Alumni seduluran selawase.

Wassalamu’alaikum Wr. Wb.
Ttd, Panitia Milad SMK YPE Cilacap ke-52.
    </textarea>

    <script>
        // --- LOGIC PERSONALISASI NAMA ---
        const urlParams = new URLSearchParams(window.location.search);
        const toName = urlParams.get('to');
        const displayElement = document.getElementById('guest-name');
        const inlineElements = document.querySelectorAll('.guest-name-inline');
        
        if (toName) {
            const formattedName = decodeURIComponent(toName);
            displayElement.innerText = formattedName;
            inlineElements.forEach(el => el.innerText = formattedName);
            
            let baseText = document.getElementById('invitationText').value;
            document.getElementById('invitationText').value = baseText.replace('[NAMA]', formattedName);
        }

        // --- COUNTDOWN TIMER ---
        const eventDate = new Date(2026, 1, 3, 7, 30); 
        function updateCountdown() {
            const now = new Date().getTime();
            const distance = eventDate - now;
            if (distance < 0) {
                document.getElementById("countdown").innerHTML = '<div class="col-span-4 text-amber-500 font-bold text-sm uppercase">ACARA SEDANG BERLANGSUNG!</div>';
                return;
            }
            const days = Math.floor(distance / (1000 * 60 * 60 * 24));
            const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((distance % (1000 * 60)) / 1000);

            const units = [days, hours, minutes, seconds];
            const labels = ['Hari', 'Jam', 'Menit', 'Detik'];
            document.getElementById("countdown").innerHTML = units.map((u, i) => `
                <div class="bg-slate-800 rounded-lg p-2 border border-slate-700">
                    <div class="text-xl font-bold text-amber-400 font-mono">${u}</div>
                    <div class="text-[10px] text-slate-500 uppercase">${labels[i]}</div>
                </div>
            `).join('');
        }
        setInterval(updateCountdown, 1000);
        updateCountdown();

        // --- ACTIONS ---
        function openMap() { window.open("https://maps.google.com/?q=Jl.+Dr.+Sutomo+No.+8+Cilacap", "_blank"); }
        function confirmWA() {
            const name = toName ? decodeURIComponent(toName) : "Tamu Undangan";
            const msg = `Halo Panitia, saya ${name} ingin konfirmasi hadir di acara Milad SMK YPE Cilacap ke-52.`;
            window.open(`https://wa.me/628112993809?text=${encodeURIComponent(msg)}`, "_blank");
        }
        function copyInvitation() {
            const text = document.getElementById('invitationText').value;
            if (navigator.clipboard) {
                navigator.clipboard.writeText(text).then(showFeedback);
            } else {
                const ta = document.createElement("textarea"); ta.value = text; document.body.appendChild(ta); ta.select(); document.execCommand('copy'); document.body.removeChild(ta); showFeedback();
            }
        }
        function showFeedback() {
            const f = document.getElementById('copyFeedback'); f.classList.remove('hidden'); setTimeout(() => f.classList.add('hidden'), 3000);
        }
    </script>
</body>
</html>
