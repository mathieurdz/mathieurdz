<!-- CÓDIGO DE LA TARJETA DE PERFIL - COPIAR Y PEGAR EN TU README.md -->
<svg width="800" height="260" viewBox="0 0 800 260" fill="none" xmlns="http://www.w3.org/2000/svg">
    <!-- DEFINICIONES: Gradientes, filtros y máscaras -->
    <defs>
        <!-- Gradiente de fondo -->
        <linearGradient id="bg-gradient" x1="0%" y1="0%" x2="100%" y2="100%">
            <stop offset="0%" style="stop-color:#111523; stop-opacity:1" />
            <stop offset="100%" style="stop-color:#0d1117; stop-opacity:1" />
        </linearGradient>
        
        <!-- Filtro de brillo para el hover de los botones -->
        <filter id="glow" x="-150%" y="-150%" width="300%" height="300%">
            <feDropShadow dx="0" dy="0" stdDeviation="6" flood-color="#a855f7" flood-opacity="0.8"/>
        </filter>

        <!-- Máscara circular para la foto de perfil -->
        <clipPath id="avatarClip">
            <circle cx="120" cy="130" r="60" />
        </clipPath>
    </defs>

    <!-- ESTILOS CSS -->
    <style>
        /* Tipografía principal */
        .card-container {
            font-family: 'Segoe UI', 'Roboto', 'Ubuntu', 'Helvetica Neue', sans-serif;
        }
        
        /* Estilos de texto */
        .name { 
            font-size: 32px; 
            font-weight: 700; 
            fill: #e0e0e0; 
        }
        .username { 
            font-size: 18px; 
            font-weight: 500; 
            fill: #8b5cf6; /* violeta */
        }
        .bio { 
            font-size: 16px; 
            font-weight: 400; 
            fill: #a0aec0; /* gris claro */
        }

        /* Estilos de los botones */
        .social-btn {
            cursor: pointer;
            transition: transform 0.2s ease-out, filter 0.2s ease-out;
        }
        .social-btn:hover {
            transform: translateY(-4px);
            filter: url(#glow);
        }
        .btn-bg {
            fill: #2a2f42;
            stroke: #4a4f66;
            stroke-width: 1;
            rx: 10; /* bordes redondeados */
            transition: fill 0.2s ease-out, stroke 0.2s ease-out;
        }
        .social-btn:hover .btn-bg {
            fill: #3c3f59;
            stroke: #a855f7;
        }
        .icon {
            fill: #cbd5e0; /* color del icono */
            transition: fill 0.2s ease-out;
        }
        .social-btn:hover .icon {
            fill: #ffffff;
        }

    </style>

    <!-- ESTRUCTURA DEL SVG -->
    <g class="card-container">
        <!-- Fondo de la tarjeta -->
        <rect width="800" height="260" fill="url(#bg-gradient)" rx="15" />
        <rect width="799" height="259" x="0.5" y="0.5" rx="14.5" stroke="#373b4d" stroke-opacity="0.6"/>

        <!-- Foto de perfil -->
        <!-- CAMBIAR: El href debe ser la URL de tu imagen. La de GitHub es ideal. -->
        <image href="https://avatars.githubusercontent.com/u/1024025?v=4" <!-- Sustituir '1024025' por tu ID de usuario de GH -->
            width="120" height="120" x="60" y="70"
            clip-path="url(#avatarClip)" />
        <circle cx="120" cy="130" r="62" fill="none" stroke="#8b5cf6" stroke-width="2" />

        <!-- Textos: Nombre, Usuario y Bio -->
        <text x="220" y="85" class="name">MATHIEUZ RDZ</text>
        <text x="220" y="115" class="username">@mathieuz-rdz</text>
        <text x="220" y="150" class="bio">Low-Level Code Alchemist | Systems Programmer & Performance Enthusiast.</text>
        <text x="220" y="175" class="bio">Crafting elegant solutions in Silicon.</text>


        <!-- Botones de Redes Sociales (Contenedor) -->
        <g transform="translate(480, 200)">
            <!-- CAMBIAR: Pon tus enlaces reales en cada `href` -->
            
            <!-- Botón 1: GitHub -->
            <a href="https://github.com/mathieuz-rdz" target="_blank" class="social-btn">
                <g transform="translate(0, 0)">
                    <rect class="btn-bg" width="50" height="50" />
                    <path class="icon" transform="translate(9, 9) scale(1.3)" d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
                </g>
            </a>

            <!-- Botón 2: LinkedIn -->
            <a href="https://linkedin.com/in/mathieuz-rdz" target="_blank" class="social-btn">
                <g transform="translate(65, 0)">
                    <rect class="btn-bg" width="50" height="50"/>
                    <path class="icon" transform="translate(13, 13) scale(1)" d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/>
                </g>
            </a>
            
            <!-- Botón 3: Twitter/X -->
            <a href="https://twitter.com/mathieuz_rdz" target="_blank" class="social-btn">
                <g transform="translate(130, 0)">
                    <rect class="btn-bg" width="50" height="50"/>
                    <path class="icon" transform="translate(13, 13) scale(1)" d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24h-6.62l-5.21-6.817L4.99 21.75H1.68l7.73-8.835L1 2.25h6.784l4.72 6.23L18.244 2.25zM17.06 19.75h1.693L7.045 4.125H5.21l11.85 15.625z"/>
                </g>
            </a>
            
            <!-- Botón 4: Mail -->
            <a href="mailto:mathieuz.dev@gmail.com" target="_blank" class="social-btn">
                <g transform="translate(195, 0)">
                    <rect class="btn-bg" width="50" height="50"/>
                    <path class="icon" transform="translate(13, 13) scale(1)" d="M0 3v18h24v-18h-24zm6.623 7.929l-6.623 5.712v-9.458l6.623 3.746zm-4.141-5.929h19.035l-9.517 7.713-9.518-7.713zm5.694 7.188l3.824 3.099 3.83-3.104 5.612 4.817h-18.779l5.513-4.812zm9.208-1.264l6.618-5.69v9.45l-6.618-3.76z"/>
                </g>
            </a>
        </g>
    </g>
</svg>
