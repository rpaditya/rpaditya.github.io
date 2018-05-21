sources=ctools-system ctools-envs ctools-overview ctools-backup ctstats ctstats-simple ctools-system-pres
#sources=lessons
testcources=ctload ctools
dest=svg png

full:
	for s in $(sources); do \
		echo processing $$s; \
		for t in $(dest); do \
			dot -T$$t $$s.dot  | sed 's/font-size:14.00/font-size:9.00/g' > $$s.$$t ; \
		done \
	done



ctload:
	dot -Tsvg ctload.dot | sed 's/font-size:14.00/font-size:11.00/g' > ctload3.svg

ctools:
	dot -Tsvg ctools.dot > ctools.svg

ctools-overview:
	dot -Tsvg ctools-overview.dot | sed 's/font-size:14.00/font-size:9.00/g' > ctools-overview.svg

ctools-backup:
	dot -Tsvg ctools-backup.dot | sed 's/font-size:14.00/font-size:9.00/g' > ctools-backup.svg

ctstats:
	dot -Tsvg ctstats.dot | sed 's/font-size:14.00/font-size:9.00/g' > ctstats.svg
	dot -Tsvg ctstats-simple.dot | sed 's/font-size:14.00/font-size:9.00/g' > ctstats-simple.svg
