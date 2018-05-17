## public Startup
```
        public void ConfigureServices(IServiceCollection services)
        {
            services.AddMvc();
            services.Configure<AppConfig>(Configuration);
            services.AddScoped<AuthenticationFilterAttribute>();
            services.AddSingleton<IPersonRepository, PersonRepository>();
        }
```
