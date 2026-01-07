<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Herramientas Informáticas - Clase Maestra</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Play:wght@400;700&family=Share+Tech+Mono&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        cyber: {
                            dark: '#050a14',
                            blue: '#0f172a',
                            fuchsia: '#d946ef',
                            red: '#ef4444',
                            dim: 'rgba(217, 70, 239, 0.1)'
                        }
                    },
                    fontFamily: {
                        play: ['Play', 'sans-serif'],
                        mono: ['Share Tech Mono', 'monospace'],
                    },
                    animation: {
                        'pulse-fast': 'pulse 1.5s cubic-bezier(0.4, 0, 0.6, 1) infinite',
                    }
                }
            }
        }
    </script>
    <style>
        body {
            background-color: #020408;
            background-image: 
                linear-gradient(rgba(5, 10, 20, 0.9), rgba(5, 10, 20, 0.9)),
                url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23d946ef' fill-opacity='0.05'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
            color: #e2e8f0;
        }

        ::-webkit-scrollbar { width: 8px; }
        ::-webkit-scrollbar-track { background: #0f172a; }
        ::-webkit-scrollbar-thumb { background: #d946ef; border-radius: 4px; }

        .crt::before {
            content: " ";
            display: block;
            position: absolute;
            top: 0; left: 0; bottom: 0; right: 0;
            background: linear-gradient(rgba(18, 16, 16, 0) 50%, rgba(0, 0, 0, 0.1) 50%), linear-gradient(90deg, rgba(255, 0, 0, 0.03), rgba(0, 255, 0, 0.01), rgba(0, 0, 255, 0.03));
            z-index: 10;
            background-size: 100% 2px, 3px 100%;
            pointer-events: none;
        }

        .fade-in { animation: fadeIn 0.5s ease-out forwards; }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body class="font-play min-h-screen flex flex-col overflow-x-hidden selection:bg-cyber-fuchsia selection:text-white">

    <!-- Header -->
    <header class="border-b-2 border-cyber-fuchsia bg-cyber-dark sticky top-0 z-50 shadow-[0_0_20px_rgba(217,70,239,0.3)]">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <div class="flex items-center space-x-3 group cursor-pointer" onclick="loadContent('home')">
                    <div class="w-10 h-10 border-2 border-cyber-red flex items-center justify-center bg-cyber-blue group-hover:animate-pulse">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-cyber-fuchsia" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 11c0 3.517-1.009 6.799-2.753 9.571m-3.44-2.04l.054-.09A13.916 13.916 0 008 11a4 4 0 118 0c0 1.017-.07 2.019-.203 3m-2.118 6.844A21.88 21.88 0 0015.171 17m3.839 1.132c.645-2.266.99-4.659.99-7.131A8 8 0 008 4.07M3 15.364c.64-1.319 1-2.8 1-4.364 0-1.457.2-2.858.567-4.171" />
                        </svg>
                    </div>
                    <div class="flex flex-col leading-tight">
                        <span class="text-xl font-bold tracking-widest text-white group-hover:text-cyber-red transition-colors">HERRAMIENTAS</span>
                        <span class="text-xs font-mono text-cyber-fuchsia">SISTEMA_OPERATIVO v2.1</span>
                    </div>
                </div>

                <nav class="hidden md:flex space-x-6">
                    <button onclick="loadContent('historia')" class="text-sm font-bold text-gray-300 hover:text-cyber-fuchsia transition uppercase tracking-tighter border-b border-transparent hover:border-cyber-fuchsia">Historia</button>
                    <button onclick="loadContent('mision')" class="text-sm font-bold text-gray-300 hover:text-cyber-fuchsia transition uppercase tracking-tighter border-b border-transparent hover:border-cyber-fuchsia">Misión</button>
                    <button onclick="loadContent('insignia')" class="text-sm font-bold text-gray-300 hover:text-cyber-fuchsia transition uppercase tracking-tighter border-b border-transparent hover:border-cyber-fuchsia">Insignia</button>
                </nav>

                <div class="hidden lg:block font-mono text-[10px] text-cyber-fuchsia border border-cyber-fuchsia/30 px-2 py-1 bg-black/40">
                    <span class="animate-pulse">●</span> EN LÍNEA
                </div>
            </div>
        </div>
    </header>

    <!-- Main -->
    <main class="flex-grow container mx-auto px-4 py-8 flex flex-col lg:flex-row gap-6">
        
        <aside class="w-full lg:w-1/4 space-y-4">
            <div class="bg-cyber-blue/50 border border-cyber-fuchsia/40 p-4 rounded shadow-lg">
                <h3 class="text-cyber-fuchsia font-mono text-xs mb-3 border-b border-cyber-fuchsia/20 pb-1">ESTADO DEL NODO</h3>
                <div class="space-y-2 text-xs font-mono">
                    <div class="flex justify-between"><span class="text-gray-500">Usuario:</span> <span class="text-white">Invitado_01</span></div>
                    <div class="flex justify-between"><span class="text-gray-500">Nivel:</span> <span class="text-cyber-red">Acceso Total</span></div>
                    <div class="mt-4 bg-gray-900 h-1.5 w-full rounded-full overflow-hidden">
                        <div class="bg-cyber-fuchsia h-full w-2/3 animate-pulse"></div>
                    </div>
                </div>
            </div>

            <div class="bg-black/40 border-l-4 border-cyber-red p-4 rounded shadow-md">
                <p class="text-[10px] text-gray-400 font-mono leading-relaxed">
                    <span class="text-cyber-red font-bold">ADVERTENCIA:</span> Los datos mostrados en este terminal son propiedad intelectual del curso. No intentar ingeniería inversa.
                </p>
            </div>
        </aside>

        <section class="w-full lg:w-3/4 flex flex-col">
            <!-- Terminal Header -->
            <div class="bg-gray-800 rounded-t-lg flex items-center justify-between px-4 py-2 border-x-2 border-t-2 border-cyber-fuchsia">
                <div class="flex space-x-1.5">
                    <div class="w-2.5 h-2.5 rounded-full bg-red-500/80"></div>
                    <div class="w-2.5 h-2.5 rounded-full bg-yellow-500/80"></div>
                    <div class="w-2.5 h-2.5 rounded-full bg-green-500/80"></div>
                </div>
                <div class="text-[10px] font-mono text-cyber-fuchsia opacity-70 uppercase tracking-widest" id="resource-title">
                    root@terminal:~/inicio
                </div>
                <div class="w-10"></div>
            </div>

            <!-- Display Area -->
            <div class="relative flex-grow bg-cyber-dark border-x-2 border-b-2 border-cyber-fuchsia shadow-[0_0_30px_rgba(217,70,239,0.15)] rounded-b-lg overflow-hidden crt min-h-[600px]">
                <div id="content-viewer" class="w-full h-full p-4 md:p-6 overflow-y-auto">
                    <!-- Contenido Dinámico -->
                </div>
            </div>
        </section>
    </main>

    <footer class="border-t border-cyber-fuchsia/20 py-4 bg-black/60">
        <div class="container mx-auto px-4 text-center">
            <p class="text-xs font-mono text-gray-500 tracking-widest">
                TERMINAL_PORTAL // 2024 // PROYECTO HERRAMIENTAS INFORMÁTICAS
            </p>
        </div>
    </footer>

    <script>
        const resources = {
            home: {
                title: 'root@terminal:~/inicio',
                content: `
                    <div class="h-full flex flex-col justify-center items-center text-center fade-in">
                        <div class="mb-4 text-cyber-red font-mono text-sm animate-pulse tracking-widest">>>> SISTEMA INICIALIZADO <<<</div>
                        <h1 class="text-4xl md:text-6xl font-bold text-white mb-6 uppercase tracking-tighter">
                            Portal de <span class="text-cyber-fuchsia">Herramientas</span>
                        </h1>
                        <p class="text-gray-400 max-w-xl mb-10 font-mono text-sm leading-relaxed">
                            Acceso centralizado a recursos académicos, registros históricos y credenciales digitales de la clase maestra.
                        </p>
                        <div class="grid grid-cols-1 md:grid-cols-3 gap-4 w-full max-w-2xl">
                            <button onclick="loadContent('historia')" class="border border-cyber-fuchsia/40 p-4 hover:bg-cyber-fuchsia/10 transition group">
                                <span class="block text-cyber-fuchsia text-[10px] mb-1 font-mono group-hover:text-white transition">01_LOGS</span>
                                <span class="font-bold text-white">HISTORIA</span>
                            </button>
                            <button onclick="loadContent('mision')" class="border border-cyber-fuchsia/40 p-4 hover:bg-cyber-fuchsia/10 transition group">
                                <span class="block text-cyber-fuchsia text-[10px] mb-1 font-mono group-hover:text-white transition">02_EXEC</span>
                                <span class="font-bold text-white">MISIÓN</span>
                            </button>
                            <button onclick="loadContent('insignia')" class="border border-cyber-fuchsia/40 p-4 hover:bg-cyber-fuchsia/10 transition group">
                                <span class="block text-cyber-fuchsia text-[10px] mb-1 font-mono group-hover:text-white transition">03_DATA</span>
                                <span class="font-bold text-white">INSIGNIA</span>
                            </button>
                        </div>
                    </div>
                `
            },
            historia: {
                title: 'root@terminal:~/data/historia.log',
                content: `
                    <div class="fade-in space-y-6">
                        <h2 class="text-2xl font-bold text-cyber-fuchsia border-b border-cyber-fuchsia/30 pb-2 flex items-center gap-2">
                            <span class="text-white">></span> REGISTRO HISTÓRICO
                        </h2>
                        
                        <div class="w-full aspect-video border border-cyber-fuchsia/30 rounded overflow-hidden bg-black shadow-lg">
                            <iframe title="Genially Historia" frameborder="0" width="100%" height="100%" src="https://view.genially.com/695d867a9a34febab07fc736" allowfullscreen="true"></iframe>
                        </div>

                        <div class="bg-cyber-blue/30 border-l-2 border-cyber-red p-4 font-mono text-sm text-gray-300">
                            <p class="mb-2"><span class="text-cyber-red font-bold">[INFO]</span> Archivo de cronología recuperado exitosamente.</p>
                            <p>Análisis de la evolución de las herramientas digitales desde el siglo XX hasta la era de la IA.</p>
                        </div>
                    </div>
                `
            },
            mision: {
                title: 'root@terminal:~/sys/mision.conf',
                content: `
                    <div class="fade-in space-y-6">
                        <h2 class="text-2xl font-bold text-cyber-fuchsia border-b border-cyber-fuchsia/30 pb-2 flex items-center gap-2">
                            <span class="text-white">></span> MISIÓN DEL SISTEMA
                        </h2>

                        <div class="w-full aspect-video border border-cyber-fuchsia/30 rounded overflow-hidden bg-black shadow-lg">
                            <iframe title="Genially Misión" frameborder="0" width="100%" height="100%" src="https://view.genially.com/695d95fa84b1464dedf24ef5" allowfullscreen="true"></iframe>
                        </div>

                        <div class="p-6 bg-black/40 border-2 border-cyber-blue text-center italic text-gray-300 font-mono">
                            "Transformar la curiosidad tecnológica en competencia profesional para un entorno digital seguro."
                        </div>
                    </div>
                `
            },
            insignia: {
                title: 'root@terminal:~/assets/badge_v1.bin',
                content: `
                    <div class="fade-in space-y-6 flex flex-col h-full">
                        <h2 class="text-2xl font-bold text-cyber-fuchsia border-b border-cyber-fuchsia/30 pb-2 flex items-center gap-2">
                            <span class="text-white">></span> INSIGNIA DE MÉRITO
                        </h2>

                        <div class="flex-grow flex flex-col items-center justify-center">
                            <div class="w-full relative shadow-[0_0_30px_rgba(217,70,239,0.2)] rounded-lg overflow-hidden border border-cyber-fuchsia/50" style="padding-top: 54%;">
                                <iframe class="absolute inset-0 w-full h-full" src="https://www.canva.com/design/DAG9rsjB7Ps/bL_HXNkwD0rGJJOHMhd7kw/view?embed" allowfullscreen="true"></iframe>
                            </div>
                            
                            <div class="mt-8 text-center w-full">
                                <h4 class="text-white font-bold text-lg mb-2">AUDITOR LEGAL</h4>
                                <p class="text-cyber-fuchsia font-mono text-xs mb-6 uppercase tracking-widest">Acreditación: Paulina Ocampo</p>
                                
                                <button onclick="window.open('https://www.canva.com/design/DAG9rsjB7Ps/bL_HXNkwD0rGJJOHMhd7kw/view', '_blank')" class="bg-cyber-fuchsia text-white px-8 py-3 font-bold hover:bg-cyber-red transition-colors shadow-[0_0_15px_rgba(217,70,239,0.4)] uppercase text-xs tracking-widest">
                                    Verificar en Red Externa
                                </button>
                            </div>
                        </div>
                    </div>
                `
            }
        };

        function loadContent(key) {
            const viewer = document.getElementById('content-viewer');
            const title = document.getElementById('resource-title');
            
            viewer.innerHTML = `
                <div class="h-full flex items-center justify-center font-mono text-cyber-fuchsia animate-pulse">
                    > DECODIFICANDO PAQUETES...
                </div>
            `;
            
            setTimeout(() => {
                const data = resources[key];
                if(data) {
                    title.innerText = data.title;
                    viewer.innerHTML = data.content;
                    viewer.scrollTo(0, 0);
                }
            }, 400);
        }

        window.onload = () => loadContent('home');
    </script>
</body>
</html>
