<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Total Fitness Academy</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body { background: #050505; color: white; font-family: 'Arial Black', Gadget, sans-serif; }
        .bein-purple { background: linear-gradient(135deg, #4d148c 0%, #1a0a2e 100%); }
        .glass { background: rgba(255,255,255,0.05); backdrop-filter: blur(10px); border: 1px solid rgba(255,255,255,0.1); }
        .neon-glow { text-shadow: 0 0 10px #a855f7, 0 0 20px #4d148c; }
    </style>
</head>
<body class="pb-24">

    <nav class="p-5 border-b border-purple-900 flex justify-between items-center sticky top-0 bg-black/90 z-50">
        <div>
            <h1 class="font-black italic text-xl leading-none tracking-tighter">TOTAL FITNESS ACADEMY</h1>
            <p class="text-[9px] text-purple-400 font-bold tracking-[0.2em]">WORLD CUP OF AEROBICS</p>
        </div>
    </nav>

    <section class="m-4 p-6 rounded-[2rem] bein-purple border-2 border-purple-500 shadow-[0_0_30px_rgba(77,20,140,0.5)]">
        <div class="flex justify-between items-start mb-4">
            <h2 class="text-3xl font-black italic uppercase leading-none">WORLD CUP<br>2026</h2>
            <span class="bg-red-600 px-2 py-1 text-[9px] font-bold rounded animate-pulse">LIVE COUNTDOWN</span>
        </div>
        
        <p class="text-xs font-bold text-purple-200 mb-4">📍 KwaMashu L Community Hall<br>📅 July 25 | 08:00 - 20:00</p>
        
        <div class="flex justify-between text-center bg-black/40 p-4 rounded-2xl mb-6 border border-purple-800/50">
            <div><span id="d" class="block text-2xl font-black neon-glow">--</span><p class="text-[8px] uppercase text-gray-400">Days</p></div>
            <div><span id="h" class="block text-2xl font-black neon-glow">--</span><p class="text-[8px] uppercase text-gray-400">Hrs</p></div>
            <div><span id="m" class="block text-2xl font-black neon-glow">--</span><p class="text-[8px] uppercase text-gray-400">Min</p></div>
            <div><span id="s" class="block text-2xl font-black text-red-500">--</span><p class="text-[8px] uppercase text-gray-400">Sec</p></div>
        </div>

        <button onclick="window.location.href='https://wa.me/27679818629?text=I%20want%20to%20book%20a%20World%20Cup%20Ticket'" class="w-full bg-white text-black font-black py-4 rounded-full uppercase text-sm active:scale-95 transition-transform">
            BUY EVENT TICKET - R300
        </button>
    </section>

    <div class="px-4 mt-8">
        <h3 class="text-[10px] font-bold text-gray-500 uppercase mb-4 tracking-widest pl-2">Monthly Academy Fees</h3>
        <div class="space-y-3">
            <div class="glass p-5 rounded-2xl flex justify-between items-center border-l-4 border-white">
                <div><p class="font-black italic">GYM CLASSES</p><p class="text-[10px] text-gray-400 font-sans">Aerobics & Group training</p></div>
                <span class="text-xl font-black">R150</span>
            </div>
            <div class="glass p-5 rounded-2xl flex justify-between items-center border-l-4 border-purple-600">
                <div><p class="font-black italic">PERSONAL TRAINING</p><p class="text-[10px] text-gray-400 font-sans">Monthly 1-on-1 coaching</p></div>
                <span class="text-xl font-black">R300</span>
            </div>
        </div>
    </div>

    <div class="p-4 mt-8 mb-4">
        <h3 class="text-[10px] font-bold text-gray-500 uppercase mb-4 tracking-widest pl-2">Chat with our Coaches</h3>
        <div class="grid grid-cols-1 gap-2">
            <a href="https://wa.me/27679818629" class="glass p-4 rounded-xl flex justify-between items-center group">
                <span class="font-bold">Cbonza (Head Coach)</span>
                <span class="text-green-500 font-black text-xs group-hover:underline">WHATSAPP</span>
            </a>
            <a href="https://wa.me/27620296345" class="glass p-4 rounded-xl flex justify-between items-center group">
                <span class="font-bold">Lungisa</span>
                <span class="text-green-500 font-black text-xs group-hover:underline">WHATSAPP</span>
            </a>
            <a href="https://wa.me/27625600946" class="glass p-4 rounded-xl flex justify-between items-center group">
                <span class="font-bold">Linda</span>
                <span class="text-green-500 font-black text-xs group-hover:underline">WHATSAPP</span>
            </a>
        </div>
    </div>

    <p class="text-center text-[10px] text-gray-600 px-10 pb-10 uppercase">Location: 183 106341 | KwaMashu</p>

    <script>
        const target = new Date("July 25, 2026 08:00:00").getTime();
        function update() {
            const now = new Date().getTime();
            const d = target - now;
            document.getElementById("d").innerHTML = Math.floor(d / (86400000));
            document.getElementById("h").innerHTML = Math.floor((d % 86400000) / 3600000);
            document.getElementById("m").innerHTML = Math.floor((d % 3600000) / 60000);
            document.getElementById("s").innerHTML = Math.floor((d % 60000) / 1000);
        }
        setInterval(update, 1000); update();
    </script>
</body>
</html>
