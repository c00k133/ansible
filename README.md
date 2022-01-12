> Why configure stuff on my server once, and instantly forget what I did?

That was the mantra I went under when playing around on my own private server.
I fixed stuff, but didn't put down the time to write about what I did (let's be honest, documentation is not always fun).
This is when I stumbled upon [Ansible](https://www.ansible.com/) I got pretty excited: configure my server without having to configure something for the configuration system itself?
Sign me up.

---

With this repository I aim to write down my configuration patterns that I use for my server.
Every time I configure something new on it I shall update this repository such that I can (preferably) idempotently run the same setup process again and again.
Not everything that I've configured and fixed this far is in here (nor might they ever show up here), but I aim to, as diligently as possible, update this repository.

#### Goals:

- To learn a new tool for server management
- To expand my repertoire of DevOps tools
- To ease my life when it comes to looking after my ~~trainwreck~~ server

---

#### TODO:

- [ ] Create role for `httpd`.
- [ ] Create playbook for server user management.
- [ ] Integrate [Terraform with Ansible](https://www.digitalocean.com/community/tutorials/how-to-use-ansible-with-terraform-for-configuration-management).
- [x] Vagrant for testing purposes: [youtube.com/watch?v=goclfp6a2IQ&t=2016s](https://www.youtube.com/watch?v=goclfp6a2IQ&t=2016s)
