# Juan lenoardo Rivera
# 04/10//2026
# 1ra version del html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="UniDash - JAMR - Proyecto escolar">
    <title> UniDash - 🌐</title>
    <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js@4.5.0/dist/chart.umd.min.js"></script>
    <link rel="stylesheet" href="./css/theme.css">
    <link rel="stylesheet" href="./css/styles.css">
</head>
<body class="bg-slate-950 text-slate-100">
    <aside id="sidebar" class="sidebar">
        <div class="sidebar-brand">
            <div class="brand-mark">🍥</div>
            <div class="brand-subtitle">Datos Mock</div>
        </div>
        <nav class="sidebar-nav" aria-label="Navegacion Principal">
            <button class="nav-item active" data-view="dashboard">Dashboard</button>
            <button class="nav-item" data-view="tasks">Tareas</button>
            <button class="nav-item" data-view="finance">Finanzas</button>
            <button class="nav-item" data-view="analytics">Estadísticas</button>
            <button class="nav-item" data-view="currency">Divisas</button>
            <button class="nav-item" data-view="news">Noticias</button>
        </nav>
        <div class="sidebar-footer">
            <p class="text-xs text-slate-500">
            | HTML5 | TailwindCSS | JavaScript | Responsive | ChartJS | </p>
        </div>
    </aside>

    <main class="main-content">
        <header class="topbar">
            <button id="mobile-menu-button" class="icon-button lg:hidden" aria-label="Abrir menú"></button>
            <div>
                <p id="page-eyebrow" class="eyebrow">Resumen Personal</p>
                <h1 id="page-title" class="page-title">Dashboard</h1>
            </div>
            <div class="topbar-location">
                <button id="location-status">Ubicacion no detectada</button>
                <button id="detect-location-button" class="secondary-button">Detectar ubicacion</button>
            </div>
        </header>
        <section id="view-dashboard" class="view-section active">
            <div class ="hero-panel">
                <div>
                    <p class="hero-copy">Todo lo mas importante en un solo dashboard</p>
                </div>
                <div class="weather-mini-card">
                    <span id="weather-icon" class="weather-icon"></span>
                    <p id="weather-temperature" class="weather-temperature">--C°</p>
                    <p id="weather-description" class="text-smtext-slate-400">Clima Proximamente</p>
                </div>
            </div>
            <div class="metric-grid">
                <article class="metric-card">
                    <p class="metric-label">Balance</p>
                    <p id="metric-balance" class="metric-value">$0.00</p>
                    <p class="metric-helper">Ingresos Menos Egresos</p>
                </article>
                <article class="metric-card">
                    <p class="metric-label">Ingresos</p>
                    <p id="metric-income" class="metric-value">$0.00</p>
                    <p class="metric-helper">Acumulador</p>
                </article>
                <article class="metric-card">
                    <p class="metric-label">Egresos</p>
                    <p id="metric-expenses" class="metric-value">$0.00</p>
                    <p class="metric-helper">Acumulados</p>
                </article>
                <article class="metric-card">
                    <p class="metric-label">Tareas pendientes</p>
                    <p id="metric-pending" class="metric-value">0</p>
                    <p class="metric-helper"></p>
                    <p class="metric-helper"></p>
                        <span id="metric-overdue">0</span> Vencidas
                </article>
            </div>
            <div class="dashboard-grid"></div>
            <article class="panel">
                <div class="panel-heading">
                    <p class="eyebrow">Finanzas</p>
                    <h3 class="panel-title">Ingresos vs Egresos</h3>
                </div>
                <button class="link-button" data-go-view="analytics">Ver Estadisticas</button>
                <div class="chart-wrapper compact-chart">
                    <canvas id="dashboard-finance-chart"></canvas>
                </div>
            </article>
            <article class="panel">
                <div class="panel-heading">
                    <p class="eyebrow">Productividad</p>
                    <h3 class="panel-title">Tareas Pendientes</h3>
                </div>
                <button class="link-button" data-go-view="analytics">Ver Tareas</button>
                <div class="chart-wrapper compact-chart">
                    <canvas id="dashboard-task-chart" class="stack-list"></canvas>
                </div>
            </article>
            <div class="dashboard-grid"></div>
        </section>
        <section id="view-tasks" class="view-section"></section>
        <section id="view-finance" class="view-section"></section>
        <section id="view-analytics" class="view-section"></section>
        <section id="view-currency" class="view-section"> </section>
        <section id="view-news" class="view-section"></section>
    </main>

    <script type="module" src="./js/main.js"></script>
    
</body>
</html>

```