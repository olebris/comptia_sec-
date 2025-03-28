# 1.3 Technical Change Management

Created time: 25 décembre 2024 19:31
Last edited by: OLB_
Last edited time: 13 mars 2025 16:16

- Avoir un process formel de mise à jour
    - Qui
    - Quand
    - Comment
        - sandbox
        - plan de test
        - rollback / backup
- Avoir un process d’approbation des mises à jour
    - Scope of the change
    - Purpose
    - Impact / Risk
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