
all:

include ../kaldi.mk

EXTRA_CXXFLAGS += -Wno-sign-compare

TESTFILES = kaldi-lattice-test push-lattice-test minimize-lattice-test \
      determinize-lattice-pruned-test word-align-lattice-lexicon-test

OBJFILES = kaldi-lattice.o lattice-functions.o word-align-lattice.o \
	   phone-align-lattice.o word-align-lattice-lexicon.o sausages.o \
        push-lattice.o minimize-lattice.o determinize-lattice-pruned.o \
				confidence.o

LIBNAME = kaldi-lat

ADDLIBS = ../hmm/kaldi-hmm.a ../tree/kaldi-tree.a ../matrix/kaldi-matrix.a \
          ../util/kaldi-util.a ../thread/kaldi-thread.a ../base/kaldi-base.a


include ../makefiles/default_rules.mk

