<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Total Fitness Academy</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body { background: #050505; color: white; font-family: sans-serif; margin: 0; padding: 0; }
        .bein-purple { background: linear-gradient(135deg, #4d148c 0%, #1a0a2e 100%); }
        .glass { background: rgba(255,255,255,0.05); backdrop-filter: blur(10px); border: 1px solid rgba(255,255,255,0.1); }
        .neon-text { text-shadow: 0 0 10px #a855f7; }
    </style>
</head>
<body class="pb-24">

    <header class="p-6 border-b border-purple-900 flex justify-between items-center bg-black">
        <div>
            <h1 class="font-black italic text-xl uppercase leading-none">TOTAL FITNESS ACADEMY</h1>
            <p class="text-[9px] text-purple-400 tracking-widest font-bold">THE WORLD CUP OF AEROBICS</p>
        </div>
    </header>

    <section class="m-4 p-6 rounded-3xl bein-purple border border-purple-500 shadow-2xl">
        <h2 class="text-2xl font-black italic uppercase leading-none mb-1">WORLD CUP 2026</h2>
        <p class="text-[10px] font-bold text-green-400 mb-4">JULY 25 @ KWAMASHU L HALL (08:00 - 20:00)</p>
        
        <div class="flex justify-between text-center bg-black/40 p-4 rounded-2xl mb-6">
            <div><span id="days" class="block text-2xl font-black neon-text">--</span><p class="text-[8px] uppercase">Days</p></div>
            <div><span id="hours" class="block text-2xl font-black neon-text">--</span><p class="text-[8px] uppercase">Hrs</p></div>
            <div><span id="mins" class="block text-2xl font-black neon-text">--</span><p class="text-[8px] uppercase">Min</p></div>
            <div><span id="secs" class="block text-2xl font-black text-red-500">--</span><p class="text-[8px] uppercase">Sec</p></div>
        </div>

        <button onclick="window.location.href='https://wa.me/27679818629?text=I%20want%20to%20buy%20a%20World%20Cup%20Ticket'" class="w-full bg-white text-black font-black py-4 rounded-full uppercase text-sm shadow-lg">
            BUY EVENT TICKET - R300
        </button>
    </section>

    <div class="px-4 mt-8">
        <h3 class="text-xs font-bold text-gray-500 uppercase mb-4 tracking-widest">Academy Fees</h3>
        <div class="space-y-3">
            <div class="glass p-5 rounded-2xl flex justify-between items-center border-l-4 border-white">
                <div><p class="font-black italic">MONTHLY CLASSES</p><p class="text-[10px] text-gray-400">Unlimited Training</p></div>
                <span class="text-xl font-black">R150</span>
            </div>
            <div class="glass p-5 rounded-2xl flex justify-between items-center border-l-4 border-purple-500">
                <div><p class="font-black italic">PERSONAL TRAINING</p><p class="text-[10px] text-gray-400">1-on-1 Sessions</p></div>
                <span class="text-xl font-black">R300</span>
            </div>
        </div>
    </div>

    <div class="p-4 mt-6">
        <h3 class="text-xs font-bold text-gray-500 uppercase mb-4 tracking-widest">WhatsApp Your Coach</h3>
        <div class="grid grid-cols-1 gap-2">
            <a href="https://wa.me/27679818629" class="glass p-3 rounded-xl flex justify-between text-sm"><span>Cbonza</span> <span class="text-green-500 font-bold">CHAT NOW</span></a>
            <a href="https://wa.me/27620296345" class="glass p-3 rounded-xl flex justify-between text-sm"><span>Lungisa</span> <span class="text-green-500 font-bold">CHAT NOW</span></a>
            <a href="https://wa.me/27625600946" class="glass p-3 rounded-xl flex justify-between text-sm"><span>Linda</span> <span class="text-green-500 font-bold">CHAT NOW</span></a>
        </div>
    </div>

    <script>
        const targetDate = new Date("July 25, 2026 08:00:00").getTime();
        function updateTimer() {
            const now = new Date().getTime();
            const diff = targetDate - now;
            if (diff < 0) return;
            document.getElementById("days").innerText = Math.floor(diff / (1000 * 60 * 60 * 24));
            document.getElementById("hours").innerText = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            document.getElementById("mins").innerText = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
            document.getElementById("secs").innerText = Math.floor((diff % (1000 * 60)) / 1000);
        }
        setInterval(updateTimer, 1000);
        updateTimer();
    </script>
</body>
</html>
