
help:
	@IFS=$$'\n' ; \
    help_lines=(`fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\\$$//'`); \
    for help_line in $${help_lines[@]}; do \
        IFS=$$'#' ; \
        help_split=($$help_line) ; \
        help_command=`echo $${help_split[0]} | sed -e 's/^ *//' -e 's/ *$$//'` ; \
        help_info=`echo $${help_split[2]} | sed -e 's/^ *//' -e 's/ *$$//'` ; \
        printf "%-10s %s\n" $$help_command $$help_info ; \
    done
cart:## setup cart component
	@bash components/cart.sh

catalogue:## setup catalogue component
	@bash components/catalogue.sh

user:## setup user component
	@bash components/user.sh

shipping:## setup shipping component
	@bash components/shipping.sh

payment:## setup payment component
	@bash components/payment.sh

frontend:## setup frontend component
	@bash components/frontend.sh


mysql:## setup mysql components
	@bash components/mysql.sh

redis:## setup redis component
	@bash components/redis.sh

rabbitmq:## setup rabbitmq component
	@bash components/rabbitmq.sh

mongodb:## setup mongodb component
	@bash components/mongodb.sh

