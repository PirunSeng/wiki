# Authentication

## Routes
config/routes.rb | routes/web.php

```
devise_for :users | Auth::routes();
```

## Controller

#### Rails
```
before_action :authenticate_user
```
#### Laravel

```
public function __construct()
{
  $this->middleware('auth');
}
```