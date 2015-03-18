FROM vossim/dashing

RUN cd /opt/dashboard \
  && dashing install d5ece60f3e1b909a671d  # Installing jenkins widget

ADD extra_files /opt/dashboard/

CMD cd /opt/dashboard && dashing start
