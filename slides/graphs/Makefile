graphs:
	@echo Making all graphs into .svg files...
	@ls *.dot | grep -v Red-black | sed s/.dot//g | awk '{print "dot -Tsvg "$$1".dot -o "$$1".svg"}' | bash
	@ls *.dot | grep -v Red-black | sed s/.dot//g | awk '{print "dot -Tps "$$1".dot -o "$$1".ps"}' | bash
	@ls *.dot | grep -v Red-black | sed s/.dot//g | awk '{print "dot -Tpng "$$1".dot -o "$$1".png"}' | bash
	@ls *.dot | grep Red-black | sed s/.dot//g | awk '{print "dot -Tsvg -Kneato "$$1".dot -o "$$1".svg"}' | bash
	@ls *.dot | grep Red-black | sed s/.dot//g | awk '{print "dot -Tps -Kneato "$$1".dot -o "$$1".ps"}' | bash
	@ls *.dot | grep Red-black | sed s/.dot//g | awk '{print "dot -Tpng -Kneato "$$1".dot -o "$$1".png"}' | bash


clean:
	/bin/rm -f *.ps *.png *~
