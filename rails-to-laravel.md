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

## View

#### Rails
```
if user_signed_in?
  ...
end
```
#### Laravel
```
@guest
  ...
@endguest
```

## Errors

#### Rails
```
ActionView::MissingTemplate
```
#### Laravel
```
View [absolute file name expected to be rendered] not found. E.g. View [app] not found.
```
