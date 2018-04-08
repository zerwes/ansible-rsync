# ansible-rsync
rsync service on debian

vars
----

	# rsync secrets file
	rsync_secrets_file: /etc/rsyncd.secrets

	# map user => home
	rsync_users:
	  rsync: /srv/rsync

	# map rsync auth user => password
	rsync_secrets:
	  tmp: RsYnCt3mp

	# map/dict module => module parameters as map/dict
	rsync_modules:
	  tmp:
	    path: /srv/rsync/tmp/
	    comment: rsync tmp
	    use chroot: yes
	    list: true
	    uid: rsync
	    gid: rsync
	    read only: false
	    auth users: tmp

