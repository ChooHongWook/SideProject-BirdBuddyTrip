# sign

## Sign

{% swagger method="post" path="/sign/up" baseUrl="localhost:4000" summary="" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="body" name="email" type="String" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="password" type="String" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="nickname" type="String" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="gender" type="String" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="birth" type="number" required="true" %}

{% endswagger-parameter %}

{% swagger-response status="200: OK" description="ok" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="post" path="/sign/in" baseUrl="localhost:4000" summary="" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="body" name="email" type="String" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="password" type="String" required="true" %}

{% endswagger-parameter %}

{% swagger-response status="200: OK" description="token 줄게" %}
```javascript
{ cookie : AccessToken }
{
    userInfo: {
        userId,
        userImage,
        userNickname,
        loginType : "kakao or email or guest"
    }
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="post" path="/sign/out" baseUrl="localhost:4000" summary="" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="body" name="token" type="String" required="true" %}
??
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="token 줄게" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

## guest



{% swagger method="post" path="/sign/guest" baseUrl="localhost:4000" summary="" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-response status="200: OK" description="ok" %}
```javascript
{
    userId,
    guestId,
}
```
{% endswagger-response %}
{% endswagger %}
