- 👋 Hi, I’m @shankar6302
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
shankar6302/shankar6302 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
int find_nth_term(int n,int a,int b,int c)
{
  if(n==1)
  return a;
  else if(n==2)
  return b;
  else if(n==3)
  return c;
  else
  {
    return find_nth_term(n-1,a,b,c)+find_nth_term
    (n-2,a,b,c)+find_nth_term(n-3,a,b,c);
  }
  }
  int main()
  {
    int n,a,b,c;
    scanf("%d%d%d%d",&n,&a,&b,&c);
    int ans=find_nth_term(n,a,b,c);
    printf("%d",ans);
    return 0;
  }
