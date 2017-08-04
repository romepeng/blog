# blog by pelican on github pages

This is my first blog in git.
利用pelican在github上 创建blog

方法：1.在系统windows10上安装Anacoda的python3版本；
        conda create --name blog_pelican python=3.6
        conda info -e
        git bash> source activate blog_pelican
      2. pip install pelican, markdown, typogrify
      3. mkdir blog
      4. cd blog
      5. pelican-quickstart
      回答问题完成配置，建立了blog的框架。
      6. clone 主题
       git clone https://github.com/getpelican/pelican-themes.git
       vim pelicanconf.py
       i 
       THEME = 'pelican-themes/gum
       Esc :wq
       7. copy a .md example into /content
       8. make html
       ((pelican e:/blog/content/ -o e:/blog/output -s e:/blog/pelicanconfg.py))
       9.make serve
       (cd e:/blog/output/ && python -m pelican.server)
       check in web: localhost:8000
       10. cd ~/output
       git init
       git add .
       git remote add origin https://github.com/romepeng/romepeng.github.io
       git pull origin master  # very important
       git commit -m 'first blog'
       git push origin master
       11. see web : https://romepeng.github.io
      
  http://markdownpad.com/download.html
  
  http://wonux.tech/git-pelican.html
  
  http://www.xycoding.com/articles/2013/11/21/blog-create/
  
  
  
  
  ## blog by hexo
  ### hexo theme  [next](http://notes.iissnan.com/ )
  ### [next example](http://notes.iissnan.com/2016/publishing-github-pages-with-travis-ci/)
      
      
