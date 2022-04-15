```.sql
--how many crimes happened at night(3)
select count(description) from crime_scene_report where description like '%night%';
```
<img width="723" alt="Screenshot 2022-04-16 at 1 36 31" src="https://user-images.githubusercontent.com/89366347/163596856-9d68d1a1-542d-4095-a1a0-e84bfe6ead64.png">
