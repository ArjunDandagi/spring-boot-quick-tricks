# spring-boot-quick-tricks
bunch of template code to copy paste to quickly get there :) 





# Redirect and multiple mappings to single method 

```@GetMapping(value = {"/","/foo"})
    public void handleFoo(HttpServletResponse response) throws  IOException {
        response.sendRedirect("/hello");
    }
```
you can also use kinda regex 


