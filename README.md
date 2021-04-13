<img src="https://user-images.githubusercontent.com/4122172/114505899-e7943d00-9be5-11eb-887c-0b163cb148f2.png" width=500>

WORK IN PROGRESS

A self-hosted file service that lets you share downloadable files with anyone on the internet via a Google-Drive-like UI but serves all data directly from your local file system.

tunnel-drive is mostly a combination of existing software I didn't write: [filebrowser](https://github.com/filebrowser/filebrowser) for the UI and backend, and [frp](https://github.com/fatedier/frp) for tunneling to the cloud.

Note that tunnel-drive is:

* not highly-available - your personal computer has to be running for the app to be online
* not scalable - only some amount of users can use this at a time before it will slow down; I'm not sure how many
* reasonably safe - I built this so I wouldn't have to expose a port in my NAT, and the app is gated by auth, but this probably shouldn't be used for sharing sensitive / top secret data
