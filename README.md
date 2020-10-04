# spring-boot-quick-tricks
bunch of template code to copy paste to quickly get there :) 





# Redirect and multiple mappings to single method 

```@GetMapping(value = {"/","/foo"})
    public void handleFoo(HttpServletResponse response) throws  IOException {
        response.sendRedirect("/hello");
    }
    @GetMapping("/hello")
    public String hmm(){
        return "Hello";
    }
```
you can also use with [RequestPath](https://stackoverflow.com/questions/22094609/multiple-mappings-to-the-same-method-of-a-controller-in-spring)


