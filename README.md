# Abejas
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Centro de Control - José Carlos</title>
    <!-- Tailwind CSS para diseño moderno y responsivo -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            50: '#f0fdf4',
                            100: '#dcfce7',
                            500: '#22c55e',
                            600: '#16a34a',
                            700: '#15803d',
                            900: '#14532d',
                        }
                    }
                }
            }
        }
    </script>
    <!-- Google Fonts Inter -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <!-- FontAwesome para iconos -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        .custom-scrollbar::-webkit-scrollbar {
            width: 6px;
        }
        .custom-scrollbar::-webkit-scrollbar-thumb {
            background-color: #cbd5e1;
            border-radius: 4px;
        }
    </style>
</head>
<body class="bg-slate-900 text-slate-100 min-h-screen flex flex-col">

    <!-- Header / Barra Superior -->
    <header class="bg-slate-800 border-b border-slate-700 sticky top-0 z-50 shadow-md">
        <div class="max-w-7xl mx-auto px-4 py-3 flex flex-col sm:flex-row justify-between items-center gap-3">
            <div class="flex items-center space-x-3">
                <div class="bg-brand-600 text-white p-2.5 rounded-xl shadow-lg">
                    <i class="fa-solid fa-bullseye text-xl"></i>
                </div>
                <div>
                    <h1 class="text-lg font-bold tracking-tight text-white">Operación CBTa 90 (Cuauhtémoc)</h1>
                    <p class="text-xs text-slate-400">Centro de Control de José Carlos | Grupo 3D</p>
                </div>
            </div>
            <!-- Estado Rápido -->
            <div class="flex items-center gap-2 bg-slate-700/60 px-3 py-1.5 rounded-lg border border-slate-600 text-xs font-medium">
                <span class="inline-block w-2.5 h-2.5 rounded-full bg-emerald-400 animate-pulse"></span>
                <span>Meta Activa: Promedio 9.5 con tu Abuela</span>
            </div>
        </div>
    </header>

    <!-- Contenido Principal -->
    <main class="flex-1 max-w-7xl w-full mx-auto p-4 sm:p-6 grid grid-cols-1 lg:grid-cols-3 gap-6">

        <!-- Columna Izquierda: Progreso y Rutina Matutina (1 Columna en LG) -->
        <div class="space-y-6">
            
            <!-- Tarjeta 1: Medidor de Promedio -->
            <section class="bg-slate-800 rounded-2xl p-5 border border-slate-700 shadow-xl relative overflow-hidden">
                <div class="absolute -right-6 -bottom-6 text-slate-700/30 text-8xl pointer-events-none">
                    <i class="fa-solid fa-graduation-cap"></i>
                </div>
                <div class="flex justify-between items-center mb-4">
                    <h2 class="text-base font-semibold text-white flex items-center gap-2">
                        <i class="fa-solid fa-chart-line text-brand-500"></i> Progreso al Promedio 9.5
                    </h2>
                    <span class="text-xs bg-amber-500/20 text-amber-400 px-2.5 py-1 rounded-full font-semibold border border-amber-500/30">Actual: 8.5</span>
                </div>
                
                <div class="space-y-3">
                    <div>
                        <div class="flex justify-between text-sm mb-1">
                            <span class="text-slate-300">Brecha hacia el objetivo</span>
                            <span class="font-bold text-emerald-400">8.5 / 9.5</span>
                        </div>
                        <div class="w-full bg-slate-700 h-3 rounded-full overflow-hidden">
                            <div class="bg-gradient-to-r from-amber-500 to-emerald-500 h-full rounded-full transition-all duration-500" style="width: 89.4%;"></div>
                        </div>
                    </div>
                    <p class="text-xs text-slate-400 mt-2">
                        Foco rojo en materias críticas para recuperar décimas vitales en la tercera entrega de boletas.
                    </p>
                </div>

                <!-- Materias Pesadas (Foco) -->
                <div class="mt-5 pt-4 border-t border-slate-700">
                    <h3 class="text-xs font-semibold text-slate-400 uppercase tracking-wider mb-3">Materias de Alto Impacto:</h3>
                    <div class="grid grid-cols-2 gap-2 text-xs">
                        <div class="bg-slate-700/50 p-2.5 rounded-xl border border-slate-600/50 flex flex-col justify-between">
                            <span class="text-slate-300 font-medium">Poligástricas</span>
                            <span class="text-amber-400 mt-1 font-semibold"><i class="fa-solid fa-triangle-exclamation"></i> Atención</span>
                        </div>
                        <div class="bg-slate-700/50 p-2.5 rounded-xl border border-slate-600/50 flex flex-col justify-between">
                            <span class="text-slate-300 font-medium">Monogástricas/Aves</span>
                            <span class="text-amber-400 mt-1 font-semibold"><i class="fa-solid fa-triangle-exclamation"></i> Atención</span>
                        </div>
                        <div class="bg-slate-700/50 p-2.5 rounded-xl border border-slate-600/50 flex flex-col justify-between">
                            <span class="text-slate-300 font-medium">CNEyT III</span>
                            <span class="text-amber-400 mt-1 font-semibold"><i class="fa-solid fa-triangle-exclamation"></i> Atención</span>
                        </div>
                        <div class="bg-slate-700/50 p-2.5 rounded-xl border border-slate-600/50 flex flex-col justify-between">
                            <span class="text-slate-300 font-medium">Temas de Literatura</span>
                            <span class="text-amber-400 mt-1 font-semibold"><i class="fa-solid fa-triangle-exclamation"></i> Atención</span>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Tarjeta 2: Rutina Matutina 5:15 AM -->
            <section class="bg-slate-800 rounded-2xl p-5 border border-slate-700 shadow-xl">
                <div class="flex justify-between items-center mb-4">
                    <h2 class="text-base font-semibold text-white flex items-center gap-2">
                        <i class="fa-solid fa-sun text-amber-400"></i> Rutina Matutina (5:15 AM)
                    </h2>
                    <span class="text-xs bg-emerald-500/20 text-emerald-400 px-2 py-0.5 rounded-md font-medium border border-emerald-500/30">CBTa 90 Ready</span>
                </div>
                <div class="space-y-3 text-sm">
                    <div class="flex items-start gap-3 p-2.5 rounded-xl bg-slate-700/30 border border-slate-700">
                        <div class="bg-amber-500/10 text-amber-400 p-2 rounded-lg font-bold text-xs mt-0.5">05:15</div>
                        <div>
                            <p class="font-medium text-slate-200">Despertar y Activación</p>
                            <p class="text-xs text-slate-400">Pliometría, fuerza y preparación física para el equipo de fútbol.</p>
                        </div>
                    </div>
                    <div class="flex items-start gap-3 p-2.5 rounded-xl bg-slate-700/30 border border-slate-700">
                        <div class="bg-amber-500/10 text-amber-400 p-2 rounded-lg font-bold text-xs mt-0.5">06:15</div>
                        <div>
                            <p class="font-medium text-slate-200">Higiene y Desayuno Energético</p>
                            <p class="text-xs text-slate-400">Nutrición adecuada para carga óptima antes de la prepa.</p>
                        </div>
                    </div>
                    <div class="flex items-start gap-3 p-2.5 rounded-xl bg-slate-700/30 border border-slate-700">
                        <div class="bg-amber-500/10 text-amber-400 p-2 rounded-lg font-bold text-xs mt-0.5">07:30</div>
                        <div>
                            <p class="font-medium text-slate-200">Salida rumbo al CBTa (Grupo 3D)</p>
                            <p class="text-xs text-slate-400">Enfoque total en clases y repaso en horas libres.</p>
                        </div>
                    </div>
                </div>
            </section>

        </div>

        <!-- Columna Central y Derecha: Horario Escolar y Tareas (2 Columnas en LG) -->
        <div class="lg:col-span-2 space-y-6">

            <!-- Tarjeta 3: Horario Escolar CBTa Grupo 3D -->
            <section class="bg-slate-800 rounded-2xl p-5 border border-slate-700 shadow-xl">
                <div class="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-3 mb-4">
                    <h2 class="text-base font-semibold text-white flex items-center gap-2">
                        <i class="fa-solid fa-calendar-days text-brand-500"></i> Horario Escolar (Grupo 3D)
                    </h2>
                    <!-- Pestañas de Días -->
                    <div class="flex bg-slate-900 p-1 rounded-xl border border-slate-700 w-full sm:w-auto overflow-x-auto">
                        <button onclick="cambiarDia('Lu')" id="btn-Lu" class="px-3 py-1.5 text-xs font-medium rounded-lg transition-all text-white bg-brand-600 shadow">Lun</button>
                        <button onclick="cambiarDia('Ma')" id="btn-Ma" class="px-3 py-1.5 text-xs font-medium rounded-lg transition-all text-slate-400 hover:text-white">Mar</button>
                        <button onclick="cambiarDia('Mi')" id="btn-Mi" class="px-3 py-1.5 text-xs font-medium rounded-lg transition-all text-slate-400 hover:text-white">Mié</button>
                        <button onclick="cambiarDia('Ju')" id="btn-Ju" class="px-3 py-1.5 text-xs font-medium rounded-lg transition-all text-slate-400 hover:text-white">Jue</button>
                        <button onclick="cambiarDia('Vi')" id="btn-Vi" class="px-3 py-1.5 text-xs font-medium rounded-lg transition-all text-slate-400 hover:text-white">Vie</button>
                    </div>
                </div>

                <!-- Contenedor de Clases por Día -->
                <div id="horario-container" class="space-y-2.5">
                    <!-- Se llena dinámicamente con JS -->
                </div>
            </section>

            <!-- Tarjeta 4: Tareas Rápidas y Pendientes Académicos -->
            <section class="bg-slate-800 rounded-2xl p-5 border border-slate-700 shadow-xl">
                <div class="flex justify-between items-center mb-4">
                    <h2 class="text-base font-semibold text-white flex items-center gap-2">
                        <i class="fa-solid fa-list-check text-brand-500"></i> Pendientes para el Promedio 9.5
                    </h2>
                    <button onclick="agregarTareaPrompt()" class="bg-brand-600 hover:bg-brand-500 text-white text-xs font-semibold px-3 py-1.5 rounded-xl transition-all shadow flex items-center gap-1.5">
                        <i class="fa-solid fa-plus"></i> Nueva Tarea
                    </button>
                </div>

                <!-- Lista de tareas interactiva -->
                <div id="lista-tareas" class="space-y-2.5 max-h-64 overflow-y-auto custom-scrollbar pr-1">
                    <!-- Se llena con JavaScript -->
                </div>
            </section>

        </div>

    </main>

    <!-- Footer Simple -->
    <footer class="bg-slate-800 border-t border-slate-700 py-4 text-center text-xs text-slate-400 mt-auto">
        <p>Centro de Control Personal - José Carlos | Diseñado para alcanzar el CBTa 90 y el 9.5 🚀</p>
    </footer>

    <!-- Script de Interactividad -->
    <script>
        // Datos del Horario del Grupo 3D basados en la imagen oficial
        const horarios3D = {
            Lu: [
                { hora: "8:00 - 9:40", materia: "Pensamiento Filosófico y Humanista III", profesor: "RCG", tipo: "normal" },
                { hora: "9:40 - 10:10", materia: "RECESO 1", profesor: "-", tipo: "receso" },
                { hora: "10:10 - 11:50", materia: "M2S2. Maneja Especies Poligástricas", profesor: "NGN", tipo: "pesada" },
                { hora: "11:50 - 12:40", materia: "CNEyT III", profesor: "LCC", tipo: "pesada" },
                { hora: "12:40 - 13:00", materia: "RECESO 2", profesor: "-", tipo: "receso" },
                { hora: "13:00 - 14:40", materia: "M2S1. Maneja Especies Monogástricas", profesor: "SLA", tipo: "pesada" }
            ],
            Ma: [
                { hora: "8:00 - 9:40", materia: "M2S2. Maneja Especies Poligástricas", profesor: "NGN", tipo: "pesada" },
                { hora: "9:40 - 10:10", materia: "RECESO 1", profesor: "-", tipo: "receso" },
                { hora: "10:10 - 11:00", materia: "Inglés III", profesor: "MMBD", tipo: "normal" },
                { hora: "11:00 - 12:40", materia: "Temas de Literatura (LyC III)", profesor: "JCA", tipo: "pesada" },
                { hora: "12:40 - 13:00", materia: "RECESO 2", profesor: "-", tipo: "receso" },
                { hora: "13:00 - 14:40", materia: "M2S3. Maneja Aves", profesor: "MLM", tipo: "pesada" }
            ],
            Mi: [
                { hora: "8:00 - 9:40", materia: "Pensamiento Filosófico y Humanista III", profesor: "RCG", tipo: "normal" },
                { hora: "9:40 - 10:10", materia: "RECESO 1", profesor: "-", tipo: "receso" },
                { hora: "10:10 - 11:00", materia: "CNEyT III", profesor: "LCC", tipo: "pesada" },
                { hora: "11:00 - 11:50", materia: "Temas de Literatura (LyC III)", profesor: "JCA", tipo: "pesada" },
                { hora: "11:50 - 12:40", materia: "Tutoría III", profesor: "PRN", tipo: "normal" },
                { hora: "12:40 - 13:00", materia: "RECESO 2", profesor: "-", tipo: "receso" },
                { hora: "13:00 - 14:40", materia: "Probabilidad y Matemáticas III", profesor: "JRO", tipo: "normal" }
            ],
            Ju: [
                { hora: "8:00 - 9:40", materia: "M2S1. Maneja Especies Monogástricas", profesor: "SLA", tipo: "pesada" },
                { hora: "9:40 - 10:10", materia: "RECESO 1", profesor: "-", tipo: "receso" },
                { hora: "10:10 - 11:50", materia: "CNEyT III", profesor: "LCC", tipo: "pesada" },
                { hora: "11:50 - 12:40", materia: "Inglés III", profesor: "MMBD", tipo: "normal" },
                { hora: "12:40 - 13:00", materia: "RECESO 2", profesor: "-", tipo: "receso" },
                { hora: "13:00 - 14:40", materia: "M2S3. Maneja Aves", profesor: "MLM", tipo: "pesada" }
            ],
            Vi: [
                { hora: "8:00 - 9:40", materia: "M2S2. Maneja Especies Poligástricas", profesor: "NGN", tipo: "pesada" },
                { hora: "9:40 - 10:10", materia: "RECESO 1", profesor: "-", tipo: "receso" },
                { hora: "10:10 - 11:00", materia: "M2S1. Maneja Especies Monogástricas", profesor: "SLA", tipo: "pesada" },
                { hora: "11:00 - 12:40", materia: "Temas de Literatura (LyC III)", profesor: "JCA", tipo: "pesada" },
                { hora: "12:40 - 13:00", materia: "RECESO 2", profesor: "-", tipo: "receso" },
                { hora: "13:00 - 14:40", materia: "Probabilidad y Matemáticas III", profesor: "JRO", tipo: "normal" }
            ]
        };

        // Estado inicial de tareas
        let tareas = [
            { id: 1, texto: "Revisar apuntes de Manejo de Especies Poligástricas", completada: false },
            { id: 2, texto: "Avanzar en los reportes pendientes de CNEyT III", completada: false },
            { id: 3, texto: "Repasar temas de Temas de Literatura / LyC III", completada: true },
            { id: 4, texto: "Preparar equipo y estiramiento para entrenamiento 5:15 AM", completada: false }
        ];

        // Cambiar vista del horario por día
        function cambiarDia(dia) {
            // Actualizar botones
            ['Lu', 'Ma', 'Mi', 'Ju', 'Vi'].forEach(d => {
                const btn = document.getElementById(`btn-${d}`);
                if (d === dia) {
                    btn.className = "px-3 py-1.5 text-xs font-medium rounded-lg transition-all text-white bg-brand-600 shadow";
                } else {
                    btn.className = "px-3 py-1.5 text-xs font-medium rounded-lg transition-all text-slate-400 hover:text-white";
                }
            });

            // Renderizar clases del día seleccionado
            const container = document.getElementById('horario-container');
            const clases = horarios3D[dia];
            
            let html = '';
            clases.forEach(c => {
                if(c.tipo === 'receso') {
                    html += `
                        <div class="bg-slate-700/20 border border-slate-700/50 p-2 rounded-xl text-center text-xs text-slate-400 font-medium">
                            <i class="fa-solid fa-mug-hot mr-1"></i> ${c.materia} (${c.hora})
                        </div>
                    `;
                } else {
                    const badgeColor = c.tipo === 'pesada' ? 'bg-amber-500/10 text-amber-400 border-amber-500/30' : 'bg-slate-700/50 text-slate-300 border-slate-600/50';
                    html += `
                        <div class="bg-slate-700/40 border border-slate-700/60 p-3 rounded-xl flex justify-between items-center text-xs sm:text-sm">
                            <div>
                                <span class="font-semibold text-white block">${c.materia}</span>
                                <span class="text-slate-400 text-xs">Prof. ${c.profesor}</span>
                            </div>
                            <div class="text-right">
                                <span class="px-2.5 py-1 rounded-lg border font-mono text-xs ${badgeColor}">${c.hora}</span>
                            </div>
                        </div>
                    `;
                }
            });
            container.innerHTML = html;
        }

        // Renderizar lista de tareas
        function renderizarTareas() {
            const container = document.getElementById('lista-tareas');
            if(tareas.length === 0) {
                container.innerHTML = `<p class="text-xs text-slate-400 text-center py-4">No hay tareas pendientes. ¡Buen trabajo!</p>`;
                return;
            }

            let html = '';
            tareas.forEach(t => {
                html += `
                    <div class="bg-slate-700/30 border border-slate-700/50 p-3 rounded-xl flex items-center justify-between gap-3 text-xs sm:text-sm">
                        <label class="flex items-center gap-3 cursor-pointer flex-1">
                            <input type="checkbox" ${t.completada ? 'checked' : ''} onclick="toggleTarea(${t.id})" class="w-4 h-4 accent-brand-500 rounded cursor-pointer">
                            <span class="${t.completada ? 'line-through text-slate-500' : 'text-slate-200'}">${t.texto}</span>
                        </label>
                        <button onclick="eliminarTarea(${t.id})" class="text-slate-500 hover:text-red-400 p-1 transition-colors">
                            <i class="fa-solid fa-trash-can text-xs"></i>
                        </button>
                    </div>
                `;
            });
            container.innerHTML = html;
        }

        function toggleTarea(id) {
            const tarea = tareas.find(t => t.id === id);
            if(tarea) {
                tarea.completada = !tarea.completada;
                renderizarTareas();
            }
        }

        function eliminarTarea(id) {
            tareas = tareas.filter(t => t.id !== id);
            renderizarTareas();
        }

        function agregarTareaPrompt() {
            const texto = prompt("Escribe el nuevo pendiente o tarea académica:");
            if(texto && texto.trim() !== "") {
                tareas.push({ id: Date.now(), texto: texto.trim(), completada: false });
                renderizarTareas();
            }
        }

        // Inicializar vista al cargar la página
        window.onload = function() {
            cambiarDia('Lu');
            renderizarTareas();
        };
    </script>
</body>
</html>