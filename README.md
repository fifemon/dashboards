Fifemon Dashboards
==================

Grafana dashboards for displaying HTCondor cluster and job information.

Expects data stored in graphite with schema:

    clusters.<cluster name>.
        collectors.
            <Name>.
                metrics...
        negotiators.
            <Name>.
                metrics...
        schedds.
            <Name>.
                metrics...
        slots.
            <SlotType>.
                <State>.
                    ...
        jobs.
            experiments.
            users.
            schedds.
            totals.
                ...

See https://github.com/fifemon/probes for scripts used to collect data.
