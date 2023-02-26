# laravel_10_adding_bootstrap5

Next steps will add BOOTSTRAP to your Laravel 10 application

1. composer require laravel/ui

2. php artisan ui bootstrap --auth

3. npm install && npm run dev

4. Open resources/js folder and check if you have this line in app.js file, if not please add line:
```
import './bootstrap';
```
5. Open resources/js folder and check if you have this line in bootstrap.js file, if not please add line :
```
import 'bootstrap';
```
6. In your resources/css/app.css file you must have:
```
@import 'bootstrap/dist/css/bootstrap.min.css';
```
7. Finally, load css and js files in your blade template
```
<!doctype html>
<html>
<head>
    <meta charset="utf-8">
    <title>{{ config('app.name', 'Laravel') }}</title>

    <!-- Scripts -->
    <script src="{{ mix('js/app.js') }}" defer></script>
    <!-- Styles -->
    <link rel="stylesheet" href="{{ mix('css/app.css') }}">
</head>
<body>
    <h1>Done</h1>
</body>
</html>
```

