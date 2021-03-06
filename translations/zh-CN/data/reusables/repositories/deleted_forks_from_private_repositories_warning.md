{% warning %}

**警告：**

- 如果您删除某人访问私有仓库的权限，则其对该私有仓库的任何复刻也会被删除。 将保留私人仓库的本地克隆。 If a team's access to a private repository is revoked or a team with access to a private repository is deleted, and team members do not have access to the repository through another team, private forks of the repository will be deleted.{% if currentVersion != "free-pro-team@latest" %}
- 当 [LDAP 同步启用](/enterprise/{{ page.version }}/admin/guides/user-management/using-ldap/#enabling-ldap-sync)后，如果从仓库删除某用户，此用户将失去访问权，但其复刻不会被删除。 如果此用户在三个月内被加入具有原组织仓库访问权限的团队，则其对复刻的访问权限将在下次同步时自动恢复。{% endif %}
- 您负责确保无法访问仓库的人员删除任何机密信息或知识产权。

- People with admin permissions to a private{% if currentVersion == "free-pro-team@latest" or currentVersion ver_gt "enterprise-server@2.19" %} or internal{% endif %} repository can disallow forking of that repository, and organization owners can disallow forking of any private{% if currentVersion == "free-pro-team@latest" or currentVersion ver_gt "enterprise-server@2.19" %} or internal{% endif %} repository in an organization. 更多信息请参阅“[管理组织的复刻政策](/github/setting-up-and-managing-organizations-and-teams/managing-the-forking-policy-for-your-organization)”和“[管理仓库的复刻政策](/github/administering-a-repository/managing-the-forking-policy-for-your-repository)”。

{% endwarning %}
