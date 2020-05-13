```yml
version: "2"
services:

  php:
    volumes:
      - your-app-files:/app:nocopy

  nginx:
    volumes:
      - your-app-files:/app:nocopy

volumes:
  your-app-files:
    external: true
```
