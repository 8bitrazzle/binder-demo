# binder-demo

1. Place your your notbook in it's own repo

2. If your code uses non standard python libraries you will need to create an environment.yml file (also placed in the root directory along with your notebook)
   This file will specify libraries for conda to install when Binder builds your notebook environment
   
   **your code only uses standard python libraries you do not need an environment.yml**

This is the contents of my environment.yml, since my notebook uses numpy and matplotlib I specify those under "dependencies"
"Name" is an orbitrary name for your environment\
"channels" specify the package manager used to install the libraries and can be kept the same
```
name: test-environment
channels:
  - conda-forge
dependencies:
  - numpy
  - matplotlib
```  
  
3. copy the clone url of your repo (in my case this is https://github.com/8bitrazzle/binder-demo.git)
4. Navigate to mybinder.org
5. Paste in the url you just copied in the first box labeled "GitHub repository name or URL"
6. Copy the url under the "Copy the URL below and share your Binder with others:" 
7. Click the orange "launch" button\
 **NOTE: The first time you do this it may take a few mintues to complete, this is normal**

Once Binder is done building your environement you can now use the url you copied in step 6 to share your notebook.
