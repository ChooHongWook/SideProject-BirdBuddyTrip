# user





{% swagger method="get" path="/user" baseUrl="localhost:4000" summary="" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="cookie" name="accessToken" required="true" %}

{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    userInfo: {
        nickname,
        image
    },
    myPost: [
    {
        postId,
        postTitle,
        postImage,
        postPeople,
        postStartDate,
        postFinishDate,
        postLike,
        postOptionGender,
        postOptionType,
        postLocation
    },{}],
    likePost: [{
        postId,
        postTitle,
        postImage,
        postPeople,
        postStartDate,
        postFinishDate,
        postLike,
        postOptionGender,
        postOptionType,
        postLocation
        },{}]
}
```
{% endswagger-response %}
{% endswagger %}



{% swagger method="put" path="/user" baseUrl="localhost:4000" summary="" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="body" name="nickname" type="String" required="false" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="password" type="String" required="false" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="image" type="String" required="false" %}

{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="delete" path="/user" baseUrl="localhost:4000" summary="" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="cookie" name="accessToken" type="String" required="true" %}

{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

## Duplicate Nickname

{% swagger method="post" path="/user/nickname" baseUrl="localhost:4000" summary="" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="body" name="nickname" type="String" required="true" %}
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

{% swagger method="post" path="/user/nickname" baseUrl="localhost:4000" summary="" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="body" name="nickname" type="String" required="true" %}
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
