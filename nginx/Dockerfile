# Образ nginx на базе alpine
FROM nginx:alpine

# Удаляем стандартный конфигурационный файл
RUN rm /etc/nginx/conf.d/default.conf

# Копируем кастомный конфигурационный файл
COPY nginx.conf /etc/nginx/nginx.conf

# Открываем порт 80
EXPOSE 80

# Запускаем nginx 
CMD ["nginx", "-g", "daemon off;"]