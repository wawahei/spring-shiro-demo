最后加一些常见的shiro异常：
1. AuthenticationException 认证异常
Shiro在登录认证过程中，认证失败需要抛出的异常。 AuthenticationException包含以下子类：

1.1. CredentitalsException 凭证异常
IncorrectCredentialsException 不正确的凭证
ExpiredCredentialsException 凭证过期

1.2. AccountException 账号异常
ConcurrentAccessException: 并发访问异常（多个用户同时登录时抛出）
UnknownAccountException: 未知的账号
ExcessiveAttemptsException: 认证次数超过限制
DisabledAccountException: 禁用的账号
LockedAccountException: 账号被锁定
UnsupportedTokenException: 使用了不支持的Token

2. AuthorizationException: 授权异常
Shiro在登录认证过程中，授权失败需要抛出的异常。 AuthorizationException包含以下子类：

2.1. UnauthorizedException:
抛出以指示请求的操作或对请求的资源的访问是不允许的。

2.2. UnanthenticatedException:
当尚未完成成功认证时，尝试执行授权操作时引发异常。

作者：王诗林
链接：https://www.jianshu.com/p/7f724bec3dc3
来源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。