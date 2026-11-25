# 02 - Gather

Extract traceable unit signals from the sources in scope.

## Input

The scope from 01.

## Process

1. Read the sources registry per [sources registry](../references/sources-registry.md).
   - Missing: say so, then offer Research plan or a manual mode where the user supplies material.
   - Material supplied: link each signal to the supplied file.
   - Both declined: stop on the Research plan offer.
2. Read each source in scope through its declared access.
   - Unreadable source: ask its owner role for an export of the scope period, take no signal from it, and go on with the readable ones.
3. Turn each item read into unit signals per [signals](../references/signals.md).
4. Count the kept signals.
   - None: report that nothing in scope holds a signal, offer the gap to Research plan per [handoffs](../references/handoffs.md), and stop.
5. Read [cluster](03-cluster.md).

## Output

The kept signals, the items dropped with their reason, and every export requested.

## Rules

- Gather writes nothing.
