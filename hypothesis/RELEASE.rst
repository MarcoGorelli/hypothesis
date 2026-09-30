RELEASE_TYPE: patch

This patch fixes :func:`~hypothesis.strategies.from_regex` for a bytes pattern
containing a negated character, such as ``rb"[^a]"``, compiled with
``re.IGNORECASE``, which previously raised an internal error.
