# filofax
Toy repository to investigate binder usage

2016-05-31 13:08:54,670 INFO: - App: Building service dependencies...
2016-05-31 13:08:54,677 INFO: - App: Copying files and filling templates...
2016-05-31 13:08:54,679 INFO: - App: Building app image without Dockerfile...
2016-05-31 13:08:54,767 INFO: - App: Sending build context to Docker daemon 58.88 kB
Sending build context to Docker daemon 58.88 kB
2016-05-31 13:08:54,818 INFO: - App: Step 0 : FROM gcr.io/generic-notebooks/binder-base
2016-05-31 13:08:54,836 INFO: - App:  ---> ec294b209d39
2016-05-31 13:08:54,864 INFO: - App: Step 1 : ADD repo $HOME/notebooks
2016-05-31 13:08:55,132 INFO: - App:  ---> dbc4b37f31d9
2016-05-31 13:08:55,184 INFO: - App: Removing intermediate container 6c72ef5ec457
2016-05-31 13:08:55,206 INFO: - App: Step 2 : USER root
2016-05-31 13:08:55,411 INFO: - App:  ---> Running in 40559fda383e
2016-05-31 13:08:55,610 INFO: - App:  ---> 5ee252217710
2016-05-31 13:08:55,618 INFO: - App: Removing intermediate container 40559fda383e
2016-05-31 13:08:55,643 INFO: - App: Step 3 : RUN chown -R main:main $HOME/notebooks
2016-05-31 13:08:55,651 INFO: - App:  ---> Running in b8a009c3a8d2
2016-05-31 13:08:56,498 INFO: - App:  ---> e37a4a649886
2016-05-31 13:08:56,503 INFO: - App: Removing intermediate container b8a009c3a8d2
2016-05-31 13:08:56,534 INFO: - App: Step 4 : USER main
2016-05-31 13:08:56,713 INFO: - App:  ---> Running in 1a0625258e98
2016-05-31 13:08:56,854 INFO: - App:  ---> 4d14cf6a2d35
2016-05-31 13:08:56,871 INFO: - App: Removing intermediate container 1a0625258e98
2016-05-31 13:08:56,938 INFO: - App: Step 5 : RUN find $HOME/notebooks -name '*.ipynb' -exec ipython trust {} \;
2016-05-31 13:08:57,041 INFO: - App:  ---> Running in 407a90e57c13
2016-05-31 13:08:57,951 INFO: - App:  ---> 84a4f94dd7ca
2016-05-31 13:08:57,958 INFO: - App: Removing intermediate container 407a90e57c13
2016-05-31 13:08:57,967 INFO: - App: Step 6 : WORKDIR $HOME/notebooks
2016-05-31 13:08:58,151 INFO: - App:  ---> Running in 0e2ef5350f00
2016-05-31 13:08:58,275 INFO: - App:  ---> 4e5f44126a6b
2016-05-31 13:08:58,307 INFO: - App: Removing intermediate container 0e2ef5350f00
2016-05-31 13:08:58,357 INFO: - App: Successfully built 4e5f44126a6b
2016-05-31 13:08:58,410 INFO: - App: Squashing and pushing gcr.io/generic-notebooks/corinnebosley-filofax to private registry...
2016-05-31 13:09:10,828 INFO: - App: Preloading app image onto all nodes...
2016-05-31 13:09:59,125 INFO: - App: Successfully built app corinnebosley-filofax
