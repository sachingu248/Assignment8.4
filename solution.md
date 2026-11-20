```html
<!DOCTYPE html>
<html>
<head>
    <title>Dashboard</title>
    <style>
        body {
            margin: 0;
            font-family: Arial;
            background: #f1f5f9;
        }

        header {
            background: #1e293b;
            color: white;
            padding: 20px;
        }

        .layout {
            display: grid;
            grid-template-columns: 200px 1fr;
            min-height: 90vh;
        }

        aside {
            background: #334155;
            color: white;
            padding: 20px;
        }

        main {
            padding: 20px;
        }

        .cards {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
        }

        .card {
            background: white;
            padding: 20px;
            border-radius: 8px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .number {
            font-size: 25px;
            color: #2563eb;
        }

        table {
            width: 100%;
            margin-top: 25px;
            background: white;
            border-collapse: collapse;
        }

        th, td {
            padding: 12px;
            border: 1px solid #ddd;
            text-align: left;
        }

        @media (max-width: 600px) {
            .layout {
                grid-template-columns: 1fr;
            }

            .cards {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>

<header><h2>My Dashboard</h2></header>

<div class="layout">
    <aside>
        <h3>Menu</h3>
        <p>Dashboard</p>
        <p>Students</p>
        <p>Courses</p>
        <p>Settings</p>
    </aside>

    <main>
        <h2>Overview</h2>

        <div class="cards">
            <div class="card"><span>👨‍🎓 Students</span><b class="number">1200</b></div>
            <div class="card"><span>📚 Courses</span><b class="number">35</b></div>
            <div class="card"><span>📝 Assignments</span><b class="number">18</b></div>
            <div class="card"><span>⏳ Pending</span><b class="number">7</b></div>
        </div>

        <h2>Recent Activity</h2>
        <table>
            <tr><th>Activity</th><th>Status</th></tr>
            <tr><td>HTML Assignment</td><td>Completed</td></tr>
            <tr><td>CSS Project</td><td>Pending</td></tr>
            <tr><td>Grid Layout</td><td>In Progress</td></tr>
        </table>
    </main>
</div>

</body>
</html>
```
