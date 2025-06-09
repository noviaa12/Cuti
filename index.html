<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sistem Informasi Cuti Pegawai - Statistik</title>
    <!-- Impor Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        primary: '#3B82F6', // Biru
                        secondary: '#10B981', // Hijau
                        danger: '#EF4444', // Merah
                        warning: '#F59E0B', // Kuning
                        info: '#6366F1', // Ungu
                        dark: '#1F2937', // Abu-abu Gelap
                    }
                }
            }
        }
    </script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        /* Custom scrollbar (opsional) */
        ::-webkit-scrollbar { width: 8px; height: 8px; }
        ::-webkit-scrollbar-track { background: #f1f1f1; border-radius: 10px; }
        ::-webkit-scrollbar-thumb { background: #888; border-radius: 10px; }
        ::-webkit-scrollbar-thumb:hover { background: #555; }

        .status-diajukan { background-color: #FEF3C7; color: #B45309; border: 1px solid #FDE68A; } /* Kuning */
        .status-disetujui { background-color: #D1FAE5; color: #065F46; border: 1px solid #A7F3D0; } /* Hijau */
        .status-ditolak { background-color: #FEE2E2; color: #991B1B; border: 1px solid #FECACA; } /* Merah */

        /* Efek hover untuk kartu statistik */
        .stat-card {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .stat-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
    </style>
</head>
<body class="bg-gray-100 font-sans">

    <!-- Header & Navigasi -->
    <header class="bg-dark shadow-lg sticky top-0 z-50">
        <div class="container mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-16">
                <div class="flex items-center">
                    <a href="#" class="text-2xl font-bold text-white">
                        <span class="text-primary">SI</span>-Cuti DP3AP2KB
                    </a>
                </div>
                <nav class="hidden md:flex space-x-4">
                    <a href="#" id="navBeranda" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Beranda</a>
                    <a href="#" id="navDaftarCuti" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Daftar Cuti</a>
                </nav>
                <div class="flex items-center">
                    <button id="openModalButton" class="bg-primary hover:bg-blue-700 text-white font-semibold py-2 px-4 rounded-lg shadow-md transition duration-300 text-sm">
                        Ajukan Cuti Baru
                    </button>
                </div>
                <!-- Mobile menu button (opsional) -->
                <div class="-mr-2 flex md:hidden">
                    <button type="button" id="mobileMenuButton" class="bg-gray-800 inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-white hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-gray-800 focus:ring-white" aria-controls="mobile-menu" aria-expanded="false">
                        <span class="sr-only">Buka menu utama</span>
                        <svg class="block h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                        </svg>
                        <svg class="hidden h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
                        </svg>
                    </button>
                </div>
            </div>
        </div>
        <!-- Mobile menu (opsional) -->
        <div class="md:hidden hidden" id="mobile-menu">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#" id="navMobileBeranda" class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium">Beranda</a>
                <a href="#" id="navMobileDaftarCuti" class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium">Daftar Cuti</a>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <main class="container mx-auto px-4 sm:px-6 lg:px-8 py-8">

        <!-- Beranda Section (Statistik) -->
        <section id="berandaSection" class="">
            <h2 class="text-3xl font-bold text-gray-800 mb-8">Dasbor Statistik Cuti</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 mb-8">
                <div class="stat-card bg-gradient-to-r from-blue-500 to-blue-600 text-white p-6 rounded-xl shadow-lg">
                    <h3 class="text-lg font-semibold mb-1">Total Pengajuan</h3>
                    <p id="statsTotalPengajuan" class="text-4xl font-bold">0</p>
                </div>
                <div class="stat-card bg-gradient-to-r from-green-500 to-green-600 text-white p-6 rounded-xl shadow-lg">
                    <h3 class="text-lg font-semibold mb-1">Disetujui</h3>
                    <p id="statsDisetujui" class="text-4xl font-bold">0</p>
                </div>
                <div class="stat-card bg-gradient-to-r from-red-500 to-red-600 text-white p-6 rounded-xl shadow-lg">
                    <h3 class="text-lg font-semibold mb-1">Ditolak</h3>
                    <p id="statsDitolak" class="text-4xl font-bold">0</p>
                </div>
                <div class="stat-card bg-gradient-to-r from-yellow-500 to-yellow-600 text-white p-6 rounded-xl shadow-lg">
                    <h3 class="text-lg font-semibold mb-1">Menunggu</h3>
                    <p id="statsMenunggu" class="text-4xl font-bold">0</p>
                </div>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <div class="bg-white p-6 rounded-xl shadow-lg">
                    <h3 class="text-xl font-semibold text-gray-700 mb-4">Ringkasan Jenis Cuti (Semua Status)</h3>
                    <div id="statsJenisCuti" class="space-y-3">
                        <!-- Statistik jenis cuti akan diisi di sini -->
                        <p class="text-sm text-gray-500">Belum ada data untuk ditampilkan.</p>
                    </div>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-lg">
                     <h3 class="text-xl font-semibold text-gray-700 mb-4">Aktivitas Terbaru</h3>
                     <ul id="aktivitasTerbaru" class="space-y-3 max-h-60 overflow-y-auto">
                        <li class="text-sm text-gray-500">Belum ada aktivitas.</li>
                     </ul>
                </div>
            </div>
        </section>

        <!-- Daftar Cuti Section -->
        <section id="daftarCutiSection" class="hidden">
            <div class="bg-white shadow-xl rounded-lg overflow-hidden">
                <div class="px-6 py-4 border-b border-gray-200 flex justify-between items-center">
                    <h2 class="text-xl font-semibold text-gray-700">Daftar Pengajuan Cuti</h2>
                    <div class="relative">
                        <input type="text" id="searchCuti" placeholder="Cari nama pegawai..." class="px-3 py-2 border border-gray-300 rounded-md shadow-sm focus:outline-none focus:ring-primary focus:border-primary sm:text-sm pl-8">
                        <svg class="w-4 h-4 text-gray-400 absolute left-2.5 top-1/2 transform -translate-y-1/2" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" />
                        </svg>
                    </div>
                </div>
                <div class="overflow-x-auto">
                    <table class="min-w-full bg-white">
                        <thead class="bg-gray-50">
                            <tr>
                                <th class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">ID</th>
                                <th class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Nama Pegawai</th>
                                <th class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Jenis Cuti</th>
                                <th class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Mulai</th>
                                <th class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Selesai</th>
                                <th class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider max-w-xs truncate">Keterangan</th>
                                <th class="px-6 py-3 text-center text-xs font-medium text-gray-500 uppercase tracking-wider">Status</th>
                                <th class="px-6 py-3 text-center text-xs font-medium text-gray-500 uppercase tracking-wider">Aksi</th>
                            </tr>
                        </thead>
                        <tbody id="tabelCuti" class="divide-y divide-gray-200">
                            <!-- Data cuti akan dimasukkan di sini -->
                        </tbody>
                    </table>
                    <div id="noDataRow" class="hidden px-6 py-10 text-center text-gray-500">
                        Belum ada data pengajuan cuti.
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-dark text-gray-400 py-6 mt-12">
        <div class="container mx-auto px-6 text-center">
            <p>&copy; <span id="currentYear"></span> Sistem Informasi Cuti Pegawai DP3AP2KB.</p>
        </div>
    </footer>

    <!-- Modal Form Pengajuan Cuti -->
    <div id="cutiModal" class="fixed inset-0 bg-gray-800 bg-opacity-75 overflow-y-auto h-full w-full flex items-center justify-center z-50 hidden">
        <div class="bg-white p-6 sm:p-8 rounded-lg shadow-2xl w-full max-w-lg mx-4 sm:mx-auto">
            <div class="flex justify-between items-center mb-6">
                <h3 class="text-xl sm:text-2xl font-semibold text-gray-800">Form Pengajuan Cuti</h3>
                <button id="closeModalButton" class="text-gray-500 hover:text-gray-700">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-7 h-7">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
                    </svg>
                </button>
            </div>
            <form id="formCuti">
                <input type="hidden" id="cutiId" name="cutiId"> <!-- Untuk mode edit -->
                <div class="mb-4">
                    <label for="namaPegawai" class="block text-sm font-medium text-gray-700 mb-1">Nama Pegawai</label>
                    <input type="text" id="namaPegawai" name="namaPegawai" class="mt-1 block w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm focus:outline-none focus:ring-primary focus:border-primary sm:text-sm" required>
                </div>
                <div class="mb-4">
                    <label for="jenisCuti" class="block text-sm font-medium text-gray-700 mb-1">Jenis Cuti</label>
                    <select id="jenisCuti" name="jenisCuti" class="mt-1 block w-full px-3 py-2 border border-gray-300 bg-white rounded-md shadow-sm focus:outline-none focus:ring-primary focus:border-primary sm:text-sm" required>
                        <option value="">Pilih Jenis Cuti...</option>
                        <option value="Cuti Tahunan">Cuti Tahunan</option>
                        <option value="Cuti Sakit">Cuti Sakit</option>
                        <option value="Cuti Alasan Penting">Cuti Alasan Penting</option>
                        <option value="Cuti Melahirkan">Cuti Melahirkan</option>
                    </select>
                </div>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mb-4">
                    <div>
                        <label for="tanggalMulai" class="block text-sm font-medium text-gray-700 mb-1">Tanggal Mulai</label>
                        <input type="date" id="tanggalMulai" name="tanggalMulai" class="mt-1 block w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm focus:outline-none focus:ring-primary focus:border-primary sm:text-sm" required>
                    </div>
                    <div>
                        <label for="tanggalSelesai" class="block text-sm font-medium text-gray-700 mb-1">Tanggal Selesai</label>
                        <input type="date" id="tanggalSelesai" name="tanggalSelesai" class="mt-1 block w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm focus:outline-none focus:ring-primary focus:border-primary sm:text-sm" required>
                    </div>
                </div>
                <div class="mb-4">
                    <label for="keterangan" class="block text-sm font-medium text-gray-700 mb-1">Keterangan</label>
                    <textarea id="keterangan" name="keterangan" rows="3" class="mt-1 block w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm focus:outline-none focus:ring-primary focus:border-primary sm:text-sm" required></textarea>
                </div>
                <div id="statusContainer" class="mb-6 hidden"> <!-- Hanya tampil saat edit -->
                     <label for="statusCuti" class="block text-sm font-medium text-gray-700 mb-1">Status</label>
                     <select id="statusCuti" name="statusCuti" class="mt-1 block w-full px-3 py-2 border border-gray-300 bg-white rounded-md shadow-sm focus:outline-none focus:ring-primary focus:border-primary sm:text-sm">
                        <option value="Diajukan">Diajukan</option>
                        <option value="Disetujui">Disetujui</option>
                        <option value="Ditolak">Ditolak</option>
                    </select>
                </div>
                <div class="flex justify-end space-x-3">
                    <button type="button" id="cancelModalButton" class="bg-gray-300 hover:bg-gray-400 text-gray-800 font-semibold py-2 px-4 rounded-lg shadow transition duration-300">
                        Batal
                    </button>
                    <button type="submit" id="submitCutiButton" class="bg-primary hover:bg-blue-700 text-white font-semibold py-2 px-4 rounded-lg shadow transition duration-300">
                        Ajukan Cuti
                    </button>
                </div>
            </form>
        </div>
    </div>

    <script>
        // --- Data & Variabel Global ---
        let daftarCuti = JSON.parse(localStorage.getItem('daftarCuti')) || [
            { id: 1, namaPegawai: "Budi Santoso", jenisCuti: "Cuti Tahunan", tanggalMulai: "2024-07-15", tanggalSelesai: "2025-07-17", keterangan: "Liburan keluarga", status: "Disetujui", diajukanPada: new Date('2024-07-10T10:00:00') },
            { id: 2, namaPegawai: "Ani Lestari", jenisCuti: "Cuti Sakit", tanggalMulai: "2024-02-01", tanggalSelesai: "2024-03-10", keterangan: "Perlu istirahat, surat dokter terlampir", status: "Diajukan", diajukanPada: new Date('2024-07-28T14:30:00') },
            { id: 3, namaPegawai: "Dinda Fitria", jenisCuti: "Cuti Alasan Penting", tanggalMulai: "2024-05-12", tanggalSelesai: "2024-05-20", keterangan: "Acara keluarga mendadak", status: "Ditolak", diajukanPada: new Date('2024-08-01T09:15:00') },
            { id: 4, namaPegawai: "Rizal Wahyu", jenisCuti: "Cuti Tahunan", tanggalMulai: "2024-09-01", tanggalSelesai: "2025-09-05", keterangan: "Refreshing", status: "Diajukan", diajukanPada: new Date('2024-08-15T11:00:00') }
        ];
        let editMode = false;
        let currentEditId = null;

        // --- Elemen DOM ---
        const berandaSection = document.getElementById('berandaSection');
        const daftarCutiSection = document.getElementById('daftarCutiSection');
        const tabelCutiBody = document.getElementById('tabelCuti');
        const noDataRow = document.getElementById('noDataRow');
        const cutiModal = document.getElementById('cutiModal');
        const openModalButton = document.getElementById('openModalButton');
        const closeModalButton = document.getElementById('closeModalButton');
        const cancelModalButton = document.getElementById('cancelModalButton');
        const formCuti = document.getElementById('formCuti');
        const cutiIdInput = document.getElementById('cutiId');
        const statusContainer = document.getElementById('statusContainer');
        const statusCutiSelect = document.getElementById('statusCuti');
        const submitCutiButton = document.getElementById('submitCutiButton');
        const searchCutiInput = document.getElementById('searchCuti');

        // Statistik Elements
        const statsTotalPengajuanEl = document.getElementById('statsTotalPengajuan');
        const statsDisetujuiEl = document.getElementById('statsDisetujui');
        const statsDitolakEl = document.getElementById('statsDitolak');
        const statsMenungguEl = document.getElementById('statsMenunggu');
        const statsJenisCutiEl = document.getElementById('statsJenisCuti');
        const aktivitasTerbaruEl = document.getElementById('aktivitasTerbaru');

        // Navigasi Elements
        const navLinks = {
            beranda: [document.getElementById('navBeranda'), document.getElementById('navMobileBeranda')],
            daftarCuti: [document.getElementById('navDaftarCuti'), document.getElementById('navMobileDaftarCuti')]
        };
        const mobileMenuButton = document.getElementById('mobileMenuButton');
        const mobileMenu = document.getElementById('mobile-menu');

        // --- Fungsi Navigasi ---
        function showSection(sectionId) {
            berandaSection.classList.add('hidden');
            daftarCutiSection.classList.add('hidden');
            document.getElementById(sectionId).classList.remove('hidden');
            updateNavActive(sectionId);
        }

        function updateNavActive(activeSectionId) {
            Object.values(navLinks).flat().forEach(link => {
                link.classList.remove('bg-gray-900', 'text-white');
                link.classList.add('text-gray-300', 'hover:bg-gray-700', 'hover:text-white');
            });
            if (activeSectionId === 'berandaSection') {
                navLinks.beranda.forEach(link => {
                    link.classList.add('bg-gray-900', 'text-white');
                    link.classList.remove('text-gray-300', 'hover:bg-gray-700', 'hover:text-white');
                });
            } else if (activeSectionId === 'daftarCutiSection') {
                 navLinks.daftarCuti.forEach(link => {
                    link.classList.add('bg-gray-900', 'text-white');
                    link.classList.remove('text-gray-300', 'hover:bg-gray-700', 'hover:text-white');
                });
            }
        }
        
        navLinks.beranda.forEach(link => link.addEventListener('click', (e) => { e.preventDefault(); showSection('berandaSection'); if(mobileMenu.classList.contains('hidden') === false) mobileMenu.classList.add('hidden'); }));
        navLinks.daftarCuti.forEach(link => link.addEventListener('click', (e) => { e.preventDefault(); showSection('daftarCutiSection'); if(mobileMenu.classList.contains('hidden') === false) mobileMenu.classList.add('hidden'); }));
        
        if (mobileMenuButton) {
            mobileMenuButton.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
                const iconOpen = mobileMenuButton.querySelector('svg:not(.hidden)');
                const iconClose = mobileMenuButton.querySelector('svg.hidden');
                iconOpen.classList.toggle('hidden');
                iconClose.classList.toggle('hidden');
            });
        }

        // --- Fungsi CRUD & Tabel ---
        function saveData() {
            localStorage.setItem('daftarCuti', JSON.stringify(daftarCuti));
        }

        function renderTabelCuti(filterNama = '') {
            tabelCutiBody.innerHTML = '';
            const filteredCuti = daftarCuti.filter(cuti => 
                cuti.namaPegawai.toLowerCase().includes(filterNama.toLowerCase())
            );

            if (filteredCuti.length === 0) {
                noDataRow.classList.remove('hidden');
                tabelCutiBody.appendChild(noDataRow.querySelector('td') ? noDataRow : createNoDataRowElement());
                return;
            }
            noDataRow.classList.add('hidden');

            filteredCuti.sort((a, b) => b.id - a.id).forEach(cuti => { // Urutkan berdasarkan ID terbaru
                const row = tabelCutiBody.insertRow();
                row.insertCell().textContent = cuti.id;
                row.insertCell().textContent = cuti.namaPegawai;
                row.insertCell().textContent = cuti.jenisCuti;
                row.insertCell().textContent = formatDate(cuti.tanggalMulai);
                row.insertCell().textContent = formatDate(cuti.tanggalSelesai);
                
                const ketCell = row.insertCell();
                ketCell.textContent = cuti.keterangan.length > 50 ? cuti.keterangan.substring(0, 50) + '...' : cuti.keterangan;
                ketCell.title = cuti.keterangan; // Tooltip untuk keterangan lengkap
                ketCell.classList.add('max-w-xs', 'truncate');


                const statusCell = row.insertCell();
                const statusBadge = document.createElement('span');
                statusBadge.textContent = cuti.status;
                statusBadge.classList.add('px-2', 'py-1', 'inline-flex', 'text-xs', 'leading-5', 'font-semibold', 'rounded-full', 'cursor-pointer');
                statusBadge.classList.add(`status-${cuti.status.toLowerCase().replace(' ', '')}`);
                statusBadge.title = `Klik untuk ubah status ${cuti.namaPegawai}`;
                statusBadge.addEventListener('click', () => openEditModal(cuti.id, true)); // Buka modal edit langsung ke status
                statusCell.appendChild(statusBadge);
                statusCell.classList.add('text-center');

                const aksiCell = row.insertCell();
                aksiCell.classList.add('text-center', 'space-x-2');
                const editButton = document.createElement('button');
                editButton.innerHTML = `<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5"><path stroke-linecap="round" stroke-linejoin="round" d="m16.862 4.487 1.687-1.688a1.875 1.875 0 1 1 2.652 2.652L10.582 16.07a4.5 4.5 0 0 1-1.897 1.13L6 18l.8-2.685a4.5 4.5 0 0 1 1.13-1.897l8.932-8.931Zm0 0L19.5 7.125M18 14v4.75A2.25 2.25 0 0 1 15.75 21H5.25A2.25 2.25 0 0 1 3 18.75V8.25A2.25 2.25 0 0 1 5.25 6H10" /></svg>`;
                editButton.classList.add('text-blue-600', 'hover:text-blue-800', 'transition', 'duration-150');
                editButton.title = "Edit Pengajuan";
                editButton.onclick = () => openEditModal(cuti.id);
                aksiCell.appendChild(editButton);

                const deleteButton = document.createElement('button');
                deleteButton.innerHTML = `<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5"><path stroke-linecap="round" stroke-linejoin="round" d="m14.74 9-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 0 1-2.244 2.077H8.084a2.25 2.25 0 0 1-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 0 0-3.478-.397m-12.56 0c1.153 0 2.24.032 3.223.094M21 12a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" /></svg>`;
                deleteButton.classList.add('text-red-600', 'hover:text-red-800', 'transition', 'duration-150');
                deleteButton.title = "Hapus Pengajuan";
                deleteButton.onclick = () => hapusCuti(cuti.id);
                aksiCell.appendChild(deleteButton);
            });
            updateStatistik();
        }

        function createNoDataRowElement() {
            const tr = document.createElement('tr');
            const td = document.createElement('td');
            td.colSpan = 8; // Sesuaikan dengan jumlah kolom
            td.className = 'px-6 py-10 text-center text-gray-500';
            td.textContent = 'Belum ada data pengajuan cuti.';
            tr.appendChild(td);
            noDataRow.innerHTML = ''; // Hapus konten lama dari #noDataRow jika ada
            noDataRow.appendChild(tr); // Masukkan baris baru
            return noDataRow;
        }
        
        function formatDate(dateString) {
            if (!dateString) return '';
            const date = new Date(dateString); // Pastikan dateString adalah format yang bisa diparse oleh Date
            const day = String(date.getDate()).padStart(2, '0');
            const month = String(date.getMonth() + 1).padStart(2, '0'); // Bulan dimulai dari 0
            const year = date.getFullYear();
            return `${day}-${month}-${year}`;
        }

        // --- Fungsi Modal ---
        function openModal(isEditMode = false, dataCuti = null, focusStatus = false) {
            editMode = isEditMode;
            formCuti.reset();
            cutiIdInput.value = '';
            statusContainer.classList.add('hidden');
            submitCutiButton.textContent = 'Ajukan Cuti';

            if (isEditMode && dataCuti) {
                currentEditId = dataCuti.id;
                cutiIdInput.value = dataCuti.id;
                document.getElementById('namaPegawai').value = dataCuti.namaPegawai;
                document.getElementById('jenisCuti').value = dataCuti.jenisCuti;
                document.getElementById('tanggalMulai').value = dataCuti.tanggalMulai;
                document.getElementById('tanggalSelesai').value = dataCuti.tanggalSelesai;
                document.getElementById('keterangan').value = dataCuti.keterangan;
                statusCutiSelect.value = dataCuti.status;
                statusContainer.classList.remove('hidden');
                submitCutiButton.textContent = 'Simpan Perubahan';
                if (focusStatus) {
                    setTimeout(() => statusCutiSelect.focus(), 0);
                }
            }
            cutiModal.classList.remove('hidden');
        }

        function closeModal() {
            cutiModal.classList.add('hidden');
            editMode = false;
            currentEditId = null;
        }
        
        openModalButton.addEventListener('click', () => openModal());
        closeModalButton.addEventListener('click', closeModal);
        cancelModalButton.addEventListener('click', closeModal);
        cutiModal.addEventListener('click', (event) => {
            if (event.target === cutiModal) closeModal();
        });

        // --- Fungsi Form Submit ---
        formCuti.addEventListener('submit', function(event) {
            event.preventDefault();
            const formData = new FormData(formCuti);
            const cutiData = {
                namaPegawai: formData.get('namaPegawai'),
                jenisCuti: formData.get('jenisCuti'),
                tanggalMulai: formData.get('tanggalMulai'),
                tanggalSelesai: formData.get('tanggalSelesai'),
                keterangan: formData.get('keterangan'),
                status: editMode ? formData.get('statusCuti') : 'Diajukan',
                diajukanPada: editMode ? daftarCuti.find(c => c.id === currentEditId).diajukanPada : new Date()
            };

            if (new Date(cutiData.tanggalSelesai) < new Date(cutiData.tanggalMulai)) {
                alert("Tanggal selesai tidak boleh sebelum tanggal mulai.");
                return;
            }

            if (editMode && currentEditId !== null) {
                const index = daftarCuti.findIndex(c => c.id === currentEditId);
                if (index > -1) {
                    daftarCuti[index] = { ...daftarCuti[index], ...cutiData, id: currentEditId };
                }
            } else {
                cutiData.id = daftarCuti.length > 0 ? Math.max(...daftarCuti.map(c => c.id)) + 1 : 1;
                daftarCuti.push(cutiData);
            }
            
            saveData();
            renderTabelCuti(searchCutiInput.value);
            updateStatistik();
            closeModal();
            alert(editMode ? "Data cuti berhasil diperbarui!" : "Pengajuan cuti berhasil ditambahkan!");
        });

        // --- Fungsi Edit & Hapus ---
        function openEditModal(id, focusStatus = false) {
            const dataCuti = daftarCuti.find(c => c.id === id);
            if (dataCuti) {
                openModal(true, dataCuti, focusStatus);
            }
        }

        function hapusCuti(id) {
            if (confirm("Apakah Anda yakin ingin menghapus pengajuan cuti ini?")) {
                daftarCuti = daftarCuti.filter(c => c.id !== id);
                saveData();
                renderTabelCuti(searchCutiInput.value);
                updateStatistik();
                alert("Data cuti berhasil dihapus.");
            }
        }
        
        // --- Fungsi Statistik ---
        function updateStatistik() {
            statsTotalPengajuanEl.textContent = daftarCuti.length;
            statsDisetujuiEl.textContent = daftarCuti.filter(c => c.status === 'Disetujui').length;
            statsDitolakEl.textContent = daftarCuti.filter(c => c.status === 'Ditolak').length;
            statsMenungguEl.textContent = daftarCuti.filter(c => c.status === 'Diajukan').length;

            // Statistik Jenis Cuti
            const jenisCutiCounts = daftarCuti.reduce((acc, cuti) => {
                acc[cuti.jenisCuti] = (acc[cuti.jenisCuti] || 0) + 1;
                return acc;
            }, {});
            
            statsJenisCutiEl.innerHTML = ''; // Clear previous stats
            if (Object.keys(jenisCutiCounts).length > 0) {
                for (const jenis in jenisCutiCounts) {
                    const percentage = ((jenisCutiCounts[jenis] / daftarCuti.length) * 100).toFixed(1);
                    const item = document.createElement('div');
                    item.innerHTML = `
                        <div class="flex justify-between items-center mb-1">
                            <span class="text-sm font-medium text-gray-600">${jenis}</span>
                            <span class="text-sm font-semibold text-primary">${jenisCutiCounts[jenis]} (${percentage}%)</span>
                        </div>
                        <div class="w-full bg-gray-200 rounded-full h-2.5">
                            <div class="bg-primary h-2.5 rounded-full" style="width: ${percentage}%"></div>
                        </div>
                    `;
                    statsJenisCutiEl.appendChild(item);
                }
            } else {
                statsJenisCutiEl.innerHTML = '<p class="text-sm text-gray-500">Belum ada data untuk ditampilkan.</p>';
            }

            // Aktivitas Terbaru
            aktivitasTerbaruEl.innerHTML = '';
            const sortedAktivitas = [...daftarCuti].sort((a,b) => new Date(b.diajukanPada) - new Date(a.diajukanPada));
            const limitAktivitas = 5;
            if(sortedAktivitas.length > 0) {
                sortedAktivitas.slice(0, limitAktivitas).forEach(cuti => {
                    const li = document.createElement('li');
                    li.classList.add('text-sm', 'p-2', 'border-b', 'border-gray-200', 'last:border-b-0');
                    const statusClass = `status-${cuti.status.toLowerCase().replace(' ', '')}`;
                    li.innerHTML = `
                        <strong>${cuti.namaPegawai}</strong> mengajukan ${cuti.jenisCuti} 
                        (<span class="${statusClass} px-1 rounded text-xs">${cuti.status}</span>) 
                        <span class="text-gray-500 block text-xs">${new Date(cuti.diajukanPada).toLocaleString('id-ID')}</span>
                    `;
                    aktivitasTerbaruEl.appendChild(li);
                });
            } else {
                aktivitasTerbaruEl.innerHTML = '<li class="text-sm text-gray-500">Belum ada aktivitas.</li>';
            }
        }

        // --- Pencarian ---
        searchCutiInput.addEventListener('input', (e) => {
            renderTabelCuti(e.target.value);
        });

        // --- Inisialisasi ---
        document.getElementById('currentYear').textContent = new Date().getFullYear();
        showSection('berandaSection'); // Tampilkan Beranda sebagai default
        renderTabelCuti(); // Render tabel awal (jika ada data dari localStorage)
        updateStatistik(); // Hitung statistik awal
    </script>
</body>
</html>
