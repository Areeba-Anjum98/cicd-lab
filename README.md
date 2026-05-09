# cicd-lab

## Canary Deployment Strategy

### Canary Deployment?
New version deployed to some users, if it is working well then it will be given to others.

### Steps:
1. **5% traffic** to new version
2. **30 minute monitor:**
   -if Error rate>1% then,rollback
   -if Response time>500ms then, rollback
3. Alright then **20% users**
4. then **50% users**
5. then **100% users**

### Monitoring:
- GitHub Actions logs check 
- Error alerts 
- Response time monitor
