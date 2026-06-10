<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portal Identitas Visitor</title>
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts: Inter -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <style>
        body { 
            font-family: 'Inter', sans-serif; 
            background-color: #f3f4f6; 
        }
        .mobile-container {
            max-width: 480px;
            margin: 0 auto;
            background-color: #ffffff;
            min-height: 100vh;
            box-shadow: 0 0 20px rgba(0,0,0,0.05);
        }
    </style>
</head>
<body class="bg-gray-100 text-gray-800 antialiased selection:bg-indigo-100 selection:text-indigo-900">

    <main class="mobile-container flex flex-col h-screen relative">
        
        <!-- App Header (Ikon Kanan Atas Sudah Dihapus) -->
        <header class="bg-white px-6 pt-8 pb-4 border-b border-gray-100 sticky top-0 z-20">
            <div>
                <h1 class="text-2xl font-bold text-gray-900 tracking-tight">Portal Identitas</h1>
                <p class="text-sm text-gray-500 font-medium">PT. BERCA NIAGA MEDIKA</p>
            </div>
        </header>

        <!-- Scrollable Content Area -->
        <div class="flex-1 overflow-y-auto p-5 bg-gray-50 flex flex-col gap-5">
            
            <!-- Digital ID Card / Header Info -->
            <div class="bg-white rounded-2xl shadow-sm border border-gray-200 overflow-hidden">
                <div class="bg-indigo-600 h-24"></div>
                <div class="px-6 pb-6 relative">
                    <div class="flex justify-between items-end -mt-12 mb-4">
                        <img id="my-photo" src="" alt="Foto Pengunjung" class="w-24 h-24 rounded-full border-4 border-white bg-white shadow-md object-cover">
                        <div class="bg-indigo-50 text-indigo-700 border border-indigo-100 px-3 py-1 rounded-full text-xs font-bold tracking-wide">
                            VISITOR
                        </div>
                    </div>
                    
                    <div>
                        <h2 id="my-name" class="text-xl font-bold text-gray-900">...</h2>
                        <p id="my-role" class="text-sm text-indigo-600 font-medium mb-1">...</p>
                        <p class="text-sm text-gray-500 flex items-center gap-1">
                            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 13.255A23.931 23.931 0 0112 15c-3.183 0-6.22-.62-9-1.745M16 6V4a2 2 0 00-2-2h-4a2 2 0 00-2 2v2m4 6h.01M5 20h14a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
                            <span id="my-company">...</span>
                        </p>
                        <p class="text-xs text-gray-400 mt-2 font-mono" id="my-id">...</p>
                    </div>
                </div>
            </div>

            <!-- Informasi Pribadi -->
            <div class="bg-white rounded-2xl shadow-sm border border-gray-200 p-5">
                <h3 class="text-sm font-bold text-gray-900 mb-4 flex items-center gap-2">
                    <svg class="w-5 h-5 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"></path></svg>
                    Identitas Pribadi
                </h3>
                <div class="grid grid-cols-2 gap-y-4 gap-x-2">
                    <div>
                        <p class="text-xs text-gray-500 mb-1">NIK</p>
                        <p id="my-nik" class="text-sm font-semibold text-gray-900">...</p>
                    </div>
                    <div>
                        <p class="text-xs text-gray-500 mb-1">Jenis Kelamin</p>
                        <p id="my-gender" class="text-sm font-semibold text-gray-900">...</p>
                    </div>
                    <div>
                        <p class="text-xs text-gray-500 mb-1">No. Handphone</p>
                        <p id="my-phone" class="text-sm font-semibold text-gray-900">...</p>
                    </div>
                    <div>
                        <p class="text-xs text-gray-500 mb-1">Email</p>
                        <p id="my-email" class="text-sm font-semibold text-gray-900 truncate">...</p>
                    </div>
                </div>
            </div>

        </div>
    </main>

    <script>
        // --- DATA PENGGUNA ---
        const userData = { 
            name: "Nuzulia Syarifah, Amd.Rad", 
            id: "VIS-20260610-001", 
            company: "RSU Islam Harapan Anda Tegal", 
            role: "Radiografer", 
            nik: "3328123456789012", 
            gender: "Perempuan", 
            phone: "0877-7469-3210", 
            email: "nuzulia.syarifah@gmail.com",
            photo: "https://placehold.co/150x150/4f46e5/ffffff?text=NS" 
        };

        // --- TAMPILKAN DATA ---
        function loadUserData() {
            // Mengisi data ke HTML berdasarkan ID
            document.getElementById('my-name').innerText = userData.name;
            document.getElementById('my-id').innerText = userData.id;
            document.getElementById('my-company').innerText = userData.company;
            document.getElementById('my-role').innerText = userData.role;
            document.getElementById('my-nik').innerText = userData.nik;
            document.getElementById('my-gender').innerText = userData.gender;
            document.getElementById('my-phone').innerText = userData.phone;
            document.getElementById('my-email').innerText = userData.email;
            document.getElementById('my-photo').src = userData.photo;
        }

        // Jalankan fungsi saat halaman dimuat
        window.onload = () => {
            loadUserData();
        };
    </script>
</body>
</html>
