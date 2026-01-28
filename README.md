<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Total Fitness Academy</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body { background: #050505; color: white; font-family: 'Arial Black', sans-serif; }
        .bein-purple { background: linear-gradient(135deg, #4d148c 0%, #1a0a2e 100%); }
        .glass { background: rgba(255,255,255,0.05); backdrop-filter: blur(10px); border: 1px solid rgba(255,255,255,0.1); }
        .neon-glow { text-shadow: 0 0 10px #a855f7; }
    </style>
</head>
<body class="pb-32">

    <header class="p-5 border-b border-purple-900 flex justify-between items-center bg-black sticky top-0 z-50">
        <div>
            <h1 class="font-black italic text-lg leading-none uppercase">TOTAL FITNESS ACADEMY</h1>
            <p class="text-[8px] text-purple-400 tracking-[0.3em] font-bold uppercase">The World Cup of Aerobics</p>
        </div>
    </header>

    <section class="m-4 p-6 rounded-[2rem] bein-purple border-2 border-purple-500 shadow-xl">
        <h2 class="text-2xl font-black italic uppercase leading-none mb-1">WORLD CUP 2026</h2>
        <p class="text-[10px] font-bold text-green-400 mb-4 uppercase">JULY 25 | KwaMashu L Hall | 08:00 - 20:00</p>
        
        <div class="flex justify-between text-center bg-black/40 p-4 rounded-2xl mb-4 border border-purple-800/50">
            <div><span id="d" class="block text-2xl font-black neon-glow">--</span><p class="text-[8px] uppercase">Days</p></div>
            <div><span id="h" class="block text-2xl font-black neon-glow">--</span><p class="text-[8px] uppercase">Hrs</p></div>
            <div><span id="m" class="block text-2xl font-black neon-glow">--</span><p class="text-[8px] uppercase">Min</p></div>
            <div><span id="s" class="block text-2xl font-black text-red-500">--</span><p class="text-[8px] uppercase">Sec</p></div>
        </div>

        <button onclick="window.location.href='https://wa.me/27679818629?text=I%20want%20to%20buy%20a%20World%20Cup%20Ticket'" class="w-full bg-white text-black font-black py-4 rounded-full uppercase text-sm shadow-lg">
            BUY EVENT TICKET - R300
        </button>
    </section>

    <div class="px-4 mt-8">
        <h3 class="text-[10px] font-bold text-gray-500 uppercase mb-4 tracking-widest pl-2">Select Your Branch</h3>
        
        <div class="space-y-4">
            <div class="glass p-4 rounded-2xl border-l-4 border-purple-600 flex items-center gap-4">
                <img src="cbonza.png" alt="Cbonza" class="w-16 h-16 rounded-full object-cover border-2 border-purple-500 bg-gray-800">
                <div class="flex-1">
                    <p class="font-black italic leading-none">KWAMASHU K SECTION</p>
                    <p class="text-[9px] text-gray-400 uppercase mt-1">Coach Cbonza</p>
                    <div class="flex gap-4 mt-2">
                        <span class="text-white text-[10px] font-bold">Classes: R150</span>
                        <span class="text-purple-400 text-[10px] font-bold">PT: R300</span>
                    </div>
                    <a href="https://wa.me/27679818629" class="text-green-500 text-[10px] font-black uppercase mt-2 inline-block underline">Chat to Book</a>
                </div>
            </div>

            <div class="glass p-4 rounded-2xl border-l-4 border-white flex items-center gap-4">
                <img src="lungisa.png" alt="Lungisa" class="w-16 h-16 rounded-full object-cover border-2 border-white bg-gray-800">
                <div class="flex-1">
                    <p class="font-black italic leading-none">E SECTION (MICHELE)</p>
                    <p class="text-[9px] text-gray-400 uppercase mt-1">Coach Lungisa (Near Bridge City)</p>
                    <div class="mt-2"><span class="text-white text-[10px] font-bold">Classes: R200</span></div>
                    <a href="https://wa.me/27620296345" class="text-green-500 text-[10px] font-black uppercase mt-2 inline-block underline">Chat to Book</a>
                </div>
            </div>

            <div class="glass p-4 rounded-2xl border-l-4 border-purple-600 flex items-center gap-4">
                <img src="linda.png" alt="Linda" class="w-16 h-16 rounded-full object-cover border-2 border-purple-500 bg-gray-800">
                <div class="flex-1">
                    <p class="font-black italic leading-none">NEWLANDS WEST</p>
                    <p class="text-[9px] text-gray-400 uppercase mt-1">Coach Linda</p>
                    <div class="mt-2"><span class="text-white text-[10px] font-bold">Classes: R250</span></div>
                    <a href="https://wa.me/27625600946" class="text-green-500 text-[10px] font-black uppercase mt-2 inline-block underline">Chat to Book</a>
                </div>
            </div>
        </div>
    </div>

    <nav class="fixed bottom-0 w-full bg-black/95 border-t border-purple-900 p-4 flex justify-around items-center z-50">
        <div class="text-center">
            <button class="text-purple-500 text-[10px] font-black uppercase">Home</button>
        </div>
        <button onclick="window.location.href='https://wa.me/27679818629'" class="bg-green-600 p-4 rounded-full -mt-12 border-4 border-black font-black text-xl shadow-lg animate-bounce">💬</button>
        <div class="text-center">
            <button onclick="alert('Video Clips coming soon!')" class="text-gray-500 text-[10px] font-black uppercase">Clips</button>
        </div>
    </nav>

    <script>
        const target = new Date("July 25, 2026 08:00:00").getTime();
        function update() {
            const now = new Date().getTime();
            const d = target - now;
            document.getElementById("d").innerText = Math.floor(d / 86400000);
            document.getElementById("h").innerText = Math.floor((d % 86400000) / 3600000);
            document.getElementById("m").innerText = Math.floor((d % 3600000) / 60000);
            document.getElementById("s").innerText = Math.floor((d % 60000) / 1000);
        }
        setInterval(update, 1000); update();
    </script>
</body>
</html>
