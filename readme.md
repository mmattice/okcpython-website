#Okc Python
---

![OKC-Python](http://i.imgur.com/SeDaFhg.png)


This is the basis for the Oklahoma City Python user group's website. This is asimply blog- type site powered by hexo, with a modified metro-lite theme. This currently supports multiple languages, and also has the ability to add plugins, as necessary.



##Updating The Site

### Getting Started

1. Make sure you have [node](http://nodejs.org/download/) installed.
2. Install hexo if you haven't already. ```npm install hexo -g```
3. Clone the repository.
  * If you already have cloned the repo, please check that your clone is up to date.
4. Run ```npm install``` from the root folder of your cloned repo.
  * Even though you've installed hexo, you must do this after the initial cloning.
5. You can start the server with ```hexo server``` on the command line.
6. Always submit news posts as a pull request. **Do not push directly to master.**
7. Full hexo documentation located at [http://hexo.io/docs/](http://hexo.io/docs/).

### Posting Events

Posts are located in _posts. The easiest way to write a new one is simply to type ```hexo new "Your Post Name"``` It will scaffold one for you. Nice.

Go ahead and Make the post you want to make. If you dont like it we can delete it later, no big deal. Now, type ```hexo server```. Hexo starts on port (in this case 4000);

When you have it like you like, do ```hexo generate``` this spits out all the static content.

### Menu
You can add a page with ```hexo new page "pagename"``` . You can add it to the menu by editing the _config.yml located in the metro-light folder

### Deploy

Easy mode. When on the master branch, after you have merged a pull request to Techlahoma's repo: ```hexo deploy --generate``` 

Boom. Its on gh pages here [http://techlahoma.github.io/okcpython-website/](http://techlahoma.github.io/okcpython-website/)



### If something goes wrong.

The magic words: ```hexo clean``` then ```hexo generate``` This will recreate everything.

*Did you forget to run* ```npm install```*?*

### Deploying for the first time ever

Basically to get the site working properly, you point your domain at the gh-pages, and the CNAME file takes care fo the rest.

1. Log into your domain registrar's website.
2. find where you admin your domain. Look for Domain Management
3. Edit your Host records like thus:

| Host Name 	| Address              	| Record Type   	| Options 	|
|-----------	|----------------------	|---------------	|---------	|
| @         	| 192.30.252.153       	| A (Address)   	|         	|
| @         	| 192.30.252.154       	| A (Address)   	|         	|
| www       	| techlahoma.github.io 	| CNAME (Alias) 	|         	|


It may take time to update.

---
Readme By : Jesse Harlin [ harlinjesse@gmail.com ]