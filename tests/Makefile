.PHONY: clean
clean:
	vagrant destroy --force

.PHONY: ssh
ssh:
	vagrant ssh -c "sudo -i"

.PHONY: vagrant-test
vagrant-test:
	vagrant up --provision

.PHONY: test-ansible22
test-ansible22:
	tox -e py27-ansible22

.PHONY: test-ansible21
test-ansible21:
	tox -e py27-ansible21

.PHONY: test
test: test-ansible22
