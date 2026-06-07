open WSL by 
	`bash`

#  go to directory:
	cd "/mnt/c/Users/admin/Desktop/MAD 2 Project/bloglite/"



[PIP error in WSL](https://stackoverflow.com/posts/55423104/timeline)

Try following command sequence on Ubuntu terminal:

```python
sudo apt-get install software-properties-common
sudo apt-add-repository universe
sudo apt-get update
sudo apt-get install python3-pip
```


# FOR CELERY WORKER
```
cd "/mnt/c/Users/admin/Desktop/MAD 2 Project/bloglite/"
source Scripts/activate
cd backend
celery -A app.celery worker -l info

```

# FOR CELERY BEAT
```
celery -A app.celery beat --max-interval 2 -l INFO
```
```
--max-interval : maximum interval to check for beat updates
```
# FOR REDIS
```
celery -A app.celery worker -l info
redis-server
```