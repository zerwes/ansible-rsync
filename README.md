# ansible-rsync
rsync service on debian

vars
----

	rsync_secrets_file: /etc/rsyncd.secrets

	rsync_secrets:
	  tmp: RsYnCt3mp

	rsync_modules:
	  tmp:
	    path: /srv/rsync/tmp/
	    comment: rsync tmp
	    use chroot: yes
	    list: true
	    uid: rsync-klaus
	    gid: rsync-klaus
	    read only: false
	    auth users: tmp

