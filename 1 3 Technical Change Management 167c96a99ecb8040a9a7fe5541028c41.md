# 1.3 Technical Change Management

Created time: 25 décembre 2024 19:31
Last edited by: OLB_
Last edited time: 4 avril 2025 13:10

- Avoir un process formel de mise à jour (procedure / SOP)
    - Qui
    - Quand
    - Comment
        - sandbox
        - plan de test
        - rollback / backup
- Avoir un process d’approbation des mises à jour
    - 1- Request the change
    - 2- Review the change
        - Scope of the change
        - Purpose
        - Impact / Risk
        - change review board or **change advisory board (CAB)**
    - 3- Approve/reject the change
    - 4- Test the change
    - 5- Schedule and implement the change
    - 6- Document the change
- Minimize the Downtime
    - repetition sur sandbox / staging
    - automatisation de la maj
    - systeme secondaire pour eviter la non dispo
- Pay attention to:
    - Restarts
    - Dependencies
    - Legacy Systems
- Documentation
    - Update Diagrams / Procedures
- Version Control (GIT)
    - Track configuration changes
    - Ability to revert
- communication
    - emails aux utilisateurs