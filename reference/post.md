# post



{% swagger method="get" path="/post?keyword=c++&max=12" baseUrl="localhost:4000" summary="" %}
{% swagger-description %}
무ㄴ 스
{% endswagger-description %}

{% swagger-parameter in="cookie" name="accessToken" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="query" name="keyword" type="String" %}
검색언어 
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    AllPost: [
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
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="get" path="/post/:id" baseUrl="localhost:4000" summary="" %}
{% swagger-description %}
id : postId
{% endswagger-description %}

{% swagger-parameter in="cookie" name="accessToken" required="true" %}

{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    AllPost: [
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
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="post" path="/post" baseUrl="localhost:4000" summary="" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="cookie" name="accessToken" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="title" type="String" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="content" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="image" required="false" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="location" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="startDate" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="finishDate" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="people" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="optionGender" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="optionType" %}

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

{% swagger method="put" path="/post/:id" baseUrl="localhost:4000" summary="" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="cookie" name="accessToken" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="title" type="String" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="content" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="image" required="false" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="location" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="startDate" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="finishDate" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="people" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="optionGender" required="true" %}

{% endswagger-parameter %}

{% swagger-parameter in="body" name="optionType" %}

{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    postId
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="delete" path="/post/:id" baseUrl="localhost:4000" summary="" %}
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
