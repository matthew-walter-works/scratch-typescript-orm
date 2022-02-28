# Tutorial
https://javascript.plainenglish.io/typeorm-tutorial-for-beginner-crud-in-express-js-typescript-b447f1fd7622

## TSOA
https://github.com/lukeautry/tsoa

## ORM
https://typeorm.io/#/

## Aspect Oriented Programming (Decorators)
- logging
- Error Handling
https://www.meziantou.net/aspect-oriented-programming-in-typescript.htm
```typescript
function sample(arg: string) {
    console.log("sample: " + arg);
    if(!isUserAuthenticated()) {
        throw new Error("User is not authenticated");
    }

    if(cache.has(arg)) {
        return cache.get(arg);
    }

    const result = 42; // TODO complex calculation
    cache.set(arg, result);
    return result;
}
```

With TypeScript, you can rewrite the method to:

```typescript
@log
@authorize
@cache
function sample(arg: string) {
    const result = 42;
    return result;
}
```

## IOC w/ TSOA
https://tsoa-community.github.io/docs/di.html#inversifyjs
https://tsoa-community.github.io/docs/di.html#tsyringe
https://tsoa-community.github.io/docs/di.html#typescript-ioc

## Creating TypeScript App
https://www.npmjs.com/package/create-express-typescript-application
