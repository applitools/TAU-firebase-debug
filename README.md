## To reproduce the crash

1. CD into functions
2. npm install
3. firebase use --add <attach it to some dummy Firebase project>
3. sudo firebase serve --only functions
4. http://localhost:5000/testproject-7ca8b/us-central1/app/hello   <--call the "hello" endpoint

In the browser you'll see:
```
{"error":{"code":500,"status":"INTERNAL","message":"function crashed","errors":["socket hang up"]}}
```

## Note:

If you do an AJAX call through a webpage, you'll see CORS error (because of this crash, although it's nothing to do with CORS and CORS is enabled)!

